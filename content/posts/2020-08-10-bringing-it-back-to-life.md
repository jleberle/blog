---
author: Jared
categories:
- Tinkering
date: "2020-08-10T10:23:00Z"
guid: https://eberlemain.nfshost.com/?p=177
id: 177
tags:
- Nerd Stuff
title: Bringing it Back to Life
url: /bringing-it-back-to-life/
---
<!-- wp:paragraph -->
<p>In 2009 or 2010 I got my first mac, a bottom of the line Mac Mini that had 2GB of RAM, a 160GB spinning disk hard drive and 2.26 Ghz processor. By 2012 the thing had run head long into the rapidly evolving computer landscape and was miserable to use, so it got replaced with an iMac that at the time had an amazing 8GB of RAM and a terabyte of storage. The Mac Mini subsequently got shuffled through a varieties of lives:</p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul><li>Sitting around just in case the new iMac crashed and I needed a backup computer</li><li>Getting brought the office in the hopes it could be used as a basic work computer. After, again, realizing the limitations of the hardware it got shuffled back home and again deposited in the lonely confines of a Rubbermaid bin full of old tech.</li><li>Serving as a single-use writing station when I lived in an apartment with no internet. It ultimately got shuffled back into storage again, but not because it failed, it was simply too much of a pain to write the stuff I needed for my dissertation at that time without internet access.</li></ul>
<!-- /wp:list -->

<!-- wp:paragraph -->
<p>For the last two plus years the Mac Mini has existed only as something to haunt the closet along with the ghosts of PS2s, a Wii, an old Apple Airport router, and countless cables I'm not entirely sure what they go to or went with. Now in the midst of a pandemic I've brought Old Chuggy back to life.[ref]I plagiarized the name from a friend's lawn guy who calls his mower Old Chuggy.[/ref]</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>My original goal this summer was essentially the same as the last time I attempted to put this computer to use: create a writing station where I could work with minimal distractions. I knew from the start I'd have to make some changes to the computer because it was after all a pre-teen and frankly ancient in computer terms. So this summer I literally popped the case and got to work.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>I updated the hard drive to a <a href="https://eshop.macsales.com/shop/ssd/owc/mac-mini/2009">solid state drive</a> and <a href="https://eshop.macsales.com/upgrades/mac-mini-late-2009-2.26-ghz/memory">upped the RAM</a> to the max of 8GB. In the end I'm still running a computer with an Intel Core 2 Duo 2.26Ghz, a very old Nvidia Graphics card, 256GB of storage, and 8GB of DDR3 RAM. There is after all, only so much you can do.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Not only did I replace the hard drive in the computer but I also changed the operating system. I long ago forgot the password I used on this computer and couldn't even boot into Mac OS X when I tried to prior to swapping hard drives, so I was going to be starting fresh. Apple officially dropped support for the 2009 Mini with the sunsetting of El Capitan in 2018, so even if I wanted to try and run MacOS, I'd probably be out of luck. Enter linux.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>My initial hope was to install <a href="https://www.archlinux.org/">Arch Linux</a> and spend some time fully customizing the install. I've played around with Arch in the past and the idea of it deeply appeals to me, especially when running an underpowered computer that would benefit from an operating system with a reduced footprint. Plus there's a wonderful community and support network through their wiki. Unfortunately when I tried booting an Arch Linux live USB it wouldn't load. Internet searching seemed to indicate it'd be a difficult prospect, so I tried Ubuntu. Same issue. The only distro I tried that would not only let me boot but also install it under the old config was Debian. Ubuntu booted and worked after replacing the hard drive and upping the RAM but I decided to stick with Debian mostly for the stability and running Debian stable would allow me to focus on working rather than tinkering with the system.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Prior to this little experiment I haven't used linux for quite some time and I'd say this is probably the most in-depth I've used any linux install I've ever done. Because my ultimate goal is to focus on work rather than tinkering I'm largely running with defaults and I've tried to keep my use of Debian backports or alternate repositories to a minimum.[ref]Currently I have evolution-ews (for Outlook support), torbrowser-launcher, <del>youtube-dl</del>, and transmission install from backports. I've added repos for NextDNS, Node, and <a href="https://typora.io/">Typora</a>.[/ref] Outside of some instances where WiFi is not recognized on some boots and some instances of lag that only resolves with a reboot, I've been pleasantly happy with the install. In the past my first chore on a fresh Debian install was to update to testing to get newer software but now I'm actually relishing using older (but still super secure and stable) software. It's doing what it needs to do, provide me an environment to work and stay out of the way of getting stuff done with bugs and errors.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>ETA: Turns out the Hugo package in Debian is both really old and problematic. Ended up using Homebrew's Linuxbrew to install the newest version. Normally at this point I'd install a bunch of other software but I'll limit myself in the spirit of this experience.[ref]I will switch youtube-dl and pandoc from official repositories to Homebrew.[/ref]</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Update: Summer 2021</strong></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>I bought a new M1 iMac and have mostly been using that at home and avoiding the office. To streamline cords I moved my old 2012 iMac to the office and replaced the Mac mini. The old iMac is running Debian stable, largely with the same setup detailed here.</p>
<!-- /wp:paragraph -->