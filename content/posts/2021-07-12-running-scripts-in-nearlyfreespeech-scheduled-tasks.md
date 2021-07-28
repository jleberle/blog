---
author: Jared
categories:
- Tinkering
date: "2021-07-12T20:04:20Z"
tags:
- Nerd Stuff
title: Running Scripts in NearlyFreeSpeech Scheduled Tasks
slug: /running-scripts-in-nearlyfreespeech-scheduled-tasks/
---
I’m not particularly smart when it comes to getting stuff to work on my web server. Eventually I’ll get there once I figure out the right Google search but usually it takes far more time than the actual problem. Take for instance the fact that I wanted to run [a script to automatically delete old tweets](https://gist.github.com/robinsloan/3688616) (via [Craig Mod]((https://daringfireball.net/thetalkshow/2021/04/11/ep-312)) but couldn’t get it to run as a scheduled task through NearlyFreeSpeech. I knew I needed a bash script wrapper for the ruby file but every time it ran it kicked back errors about not finding the needed ruby gems even though I had installed the gems. Because I’m an idiot I sent all my parameters in my bash_profile, which only works for interactive sessions (e.g. why it worked when I was logged in to a session and ran it manually), the rest of the time it pulled from the standard directories. So hours of searching was solved by defining the ruby gems paths in my wrapper script.

~~~
#!/bin/sh

export GEM_HOME=/home/private/gems
export GEM_PATH=/home/private/gems:/usr/local/lib/ruby/gems/2.7/
export PATH=$PATH:/home/private/gems/bin:/home/private/bin

exec ruby /home/private/bin/tweetdelete.rb
~~~