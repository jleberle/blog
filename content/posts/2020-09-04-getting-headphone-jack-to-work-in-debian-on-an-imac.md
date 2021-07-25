---
author: Jared
categories:
- Tinkering
date: "2020-09-04T12:56:00Z"
guid: https://eberlemain.nfshost.com/?p=220
id: 220
tags:
- Nerd Stuff
title: Getting Headphone Jack to Work in Debian on an iMac
url: /getting-headphone-jack-to-work-in-debian-on-an-imac/
---
<!-- wp:paragraph -->
<p>After desperately searching for a solution to the Debian install on my old 2012 iMac not producing sounds through the headphone jack connected speakers, <a href="https://linux-tips.com/t/how-to-fix-apple-imac-headphone-sound-problem/285">this provided the solution</a>:</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>To fix this problem, you have to load snd-hda-intel module with model=imac27_122 option.<br>To do this, create a new file (if similar conf file for snd-hda-intel module exists, use that one) for example /etc/modprobe.d/sound.conf with following content:</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>options snd-hda-intel model=imac27_122</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>and reboot, that’s all.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>I tacked my onto alsa.conf</p>
<!-- /wp:paragraph -->