---
author: Jared
categories:
- Tinkering
date: "2020-09-04T12:56:00Z"
tags:
- Nerd Stuff
title: Getting Headphone Jack to Work in Debian on an iMac
slug: /getting-headphone-jack-to-work-in-debian-on-an-imac/
original: false
author: Linux Tips
link: https://linux-tips.com/t/how-to-fix-apple-imac-headphone-sound-problem/285
---
After desperately searching for a solution to the Debian install on my old 2012 iMac not producing sounds through the headphone jack connected speakers, this provided the solution:

> To fix this problem, you have to load snd-hda-intel module with model=imac27_122 option.
>
>  To do this, create a new file (if similar conf file for snd-hda-intel module exists, use that one) for example /etc/modprobe.d/sound.conf with following content:
>
> ~~~
> options snd-hda-intel model=imac27_122
> ~~~

and reboot, that’s all.
