---
author: Jared
categories:
- Academia
date: "2016-03-21T15:43:00Z"
tags:
- Nerd Stuff
title: Publishing a Markdown CV to PDF and HTML
slug: /publishing-a-markdown-cv-to-pdf-and-html/
---
**Update:** *I still use some of this, but this is out of date. Use with caution.*

Huge caveat from the get go: I don't know how useful any of this will be to anyone. For one, there are probably far more elegant ways of doing this whole affair and someone smarter than me has undoubtedly found it. Secondly, if you're anyone who knows me personally, this is probably all crazy talk. But with that being said…

## The Problem

I like to write my CV in markdown so that I have it all in plaintext and it's easy to manage and export when needed. However, I also like to host an HTML version of my CV and also provide a PDF version for applications. The issue is that for the HTML version I like to include a link to the PDF version as well as Links to other items in the CV. These Links, however, are distracting in the PDF version. So I needed to find a way to manage two versions of the same document with relative ease. While I could just host two versions of of the CV, say cvhtml.md and cvpdf.md, both documents tend to share most of the same things, so anytime I edit large chunks of the document, I'd have to do it twice.

## The Answer (Maybe)

The answer I came up with was to break the CV up into individual parts and utilize [Markdown-PP](https://github.com/jreese/markdown-pp) to merge the files into one markdown file that could then be converted into either a PDF or an HTML file depending on which was needed. You can see the bones of the operation in [this Github repository](https://github.com/jleberle/cv). Most of it is basic, but the magic involved Markdown-PP's ability to pull files, so in the top level files, cvhtml.mdpp and cvpdf.mdpp you get bits like this:


~~~
## Publications

!INCLUDE "html/publications.mdpp"

## Conference Papers

!INCLUDE "html/conferences.mdpp" 
~~~

As a result I can maintain two seperate files for the sections that differ and one file for the sections that don't vary depending on which version I need. This still leaves me with some redundant editing, but less than I had otherwise. Adding another step, however, means typing additional commands, which undermines some of the reason for this whole affair. As such I wrote a rudimentary Rakefile to create tasks to automate this process:

~~~
require 'rake/clean'

CLEAN.include("*.md","*.html")

desc "Build html and pdf"
task :default =&gt; &#91;:makepdf, :makehtml, :clean]

desc "Build PDF version only"
task :makepdf do
  sh "markdown-pp cvpdf.mdpp -o cv.md"
  sh "pandoc cv.md -o cv.pdf"
  sh "scp cv.pdf blog:/home/public/cv"
end

desc "Build HTML only"
task :makehtml do
  sh "markdown-pp cvhtml.mdpp -o index.md"
  sh "pandoc -r markdown+simple_tables+table_captions+yaml_metadata_block -s -S -c main.css index.md -o index.html"
  sh "scp index.html blog:/home/public/cv"
end
~~~

All of that is pretty simple. The default task builds both the PDF and HTML versions of the files. The file also provides the option to build just the PDF or HTML version, but I rarely have a use for building one and not the other. Nevertheless both of the tasks do basically the same thing, build the markdown version using Markdown-PP and then converting the file to HTML or PDF with Pandoc, copying the resulting file to my server, and finally removing the development files. One thing to note, the main.css referenced in the Pandoc HTML conversion is the Lopash.css file you find in Marked 2, I just extracted it from the app and made some minor changes to the styling.

Again, is any of this useful? I don't know, but it's there anyway.
