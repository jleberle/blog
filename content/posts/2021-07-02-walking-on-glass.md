---
author: Jared
categories:
- Tinkering
date: "2021-07-02T13:18:00Z"
guid: https://eberlemain.nfshost.com/?p=131
id: 131
tags:
- Nerd Stuff
title: Walking on Glass
slug: /walking-on-glass/
---
I’ve been using the public betas of iOS/iPadOS and MacOS since they came out in the last few days and there’s a lot to love about the forthcoming releases.

I love the fact that my iPad Home Screen can now be an information screen with widgets.[^1] Apps are now either in the dock or relegated to the App Library. I don’t see much use for apps on the Home Screen at this point.

{{< figure src="/images/2021/07/ipadhome.png" >}}

I love quick note and the ability to quickly add a note from anywhere. Notes is a a subtle star within Apple’s stable of apps and in the last year it’s gone from a relatively useless app to one of the most used.

Multitasking in every version of iPadOS felt like something tacked on. It was there and semi-functional but it never felt like it was worth the bother to actually use. Because of that I never used it much and mostly interacted with popover out of annoyance when I triggered it by mistake. The updated version has the little dots at the top of the screen which serve as a nice reminder that it’s there.

All of these are the kind of improvements that make it worth it. Functional and effective workflow improvements. At the same time Apple has vastly improved in areas, they decided to take a twelve gauge and blow their whole foot off with Safari.

Chrome is the dominant browser and no one is going to catch it sadly. Apple had a solid browser that worked effectively and provided a good default option for most people. Yet the “refresh” in the new versions are a disaster. Nothing has really improved with the central app most people use but a lot has gotten much worse for no real reason.

The best new version of Safari is on the iPad and even there it’s a walk back. I can tolerate the unified tab and URL bar but whereas Quick Note makes things more accessible, Safari does the opposite. Accessing private browsing tabs, the share menu, and refreshing the page are all now more difficult:

{{< figure src="/images/2021/07/ipadsafari.png" >}}

- Private Browsing: If you have a keyboard you can invoke a window with the standard Cmd+Shift+N shortcut, otherwise you have to click the sidebar, select private browsing, and then close the sidebar if your iPad is in landscape mode. That’s three clicks to two in the current version.
- Share Menu: It’s now in the more menu. What used to be one tap is now two.
- Reload: You can invoke it with a keyboard shortcut or the more menu but the default way Apple seems to support is scrolling to the top of the page and pulling down. That’s a nice option, but the default? If I refresh a page via the keyboard it keeps my place, which can be usual when waiting for something to go on-sale. Scrolling to the top and pulling down requires you to scroll back down.

Because of the keyboard all of these are manageable on the iPad but on the iPhone everything falls apart and will cause a lot of people to consider jumping ship.

On iOS Apple fundamentally re-did the browser’s interface, moving the URL bar to the bottom and making it floating. It makes accessing the URL bar easier but everything else is much worse off:

{{< figure src="/images/2021/07/floatingbar.png" >}}
{{< figure src="/images/2021/07/minimizedbar.png" >}}

- Private Browsing: <s>Click the tabs icon, click the down arrow to access tab groups, click private browsing. Three clicks to two.</s> Edit: Long press on the tabs icon.
- Share Menu: In the more menu, two clicks to one.
- Reload: Can be accessed by the more menu but the pull to refresh is the only way without going into the menus. And sometimes it doesn’t seem to trigger.
- Reader View: This is by far the most obnoxious one because Reader View is best on smaller screens like the iPhone. When you start scrolling on a website the floating URL bar tucks down into the bottom of the screen becoming almost invisible. On first read the non-inactive bar will tell you Reader View is available, but if you click it to access it all that happens is the floating URL bar comes back. <s>In order to access Reader View you have to click the more menu, two clicks to one.</s> Edit: You can long press the more menu to get it.

What problem did Apple think they had with have these options available with a single tap? It feels like nothing more than someone’s egregious minimalist fetish that’s going to annoy a lot of people.

On the Mac Safari is okay. I can tolerate the uni-URL/tab bar with time. But the decision to enable it taking on the main background color of the tab by default is terrible. One second Safari is orange, the next red, and then blue. Sure it makes the bar disappear into the content but why do I want that? It’s disconcerting and at times unreadable. I could see it being helpful if you open a Safari window for each new tab but otherwise it’s just useless UI.[^1] You can disable it in the settings so annoying but easy to get rid of.

{{< figure src="/images/2021/07/advancedoptions.png" >}}

The other big thing in Safari is the introduction of Privacy Relay, which sends your connections through an ingress and egress server to hide your IP and browsing from websites and trackers. The ingress server knows who you are but not where you’re going, the egress server (which isn’t Apple) knows where you’re going, not who you are. The service is available if you have a paid iCloud account and is on by default, hiding your IP from websites and trackers. It doesn’t slow down browsing to a noticeable degree although I have seen a small uptick in websites making me prove I’m not a robot.[ref]It’s not as bad as a VPN but it does appear to trip up the spam protection of a few websites like Walmart.[/ref] It also conflicts with custom DNS and VPNs, things that will get ironed out as developers update the apps for the next version. Apple does allow for you to only use it for known trackers rather than websites as a whole.

Finally Apple sought to combat email tracking with an option to block trackers. Unlike something like [MailTrackerBlocker](https://apparition47.github.io/MailTrackerBlocker/) which blocks trackers outright, Apple proxies all remote content through their servers. Decide whether that's your thing or not I guess.

In essence the first impressions are that the updates make a bunch of really get steps forward but then end up in the emergency room to get the feet sown up because of a willful decision to walk through a field of broken glass. Safari and the web are still a central part of the user experience and Apple decided to make it worse in the name of making it better.

--- 
[^1]: For some reason Apple has retained the old style widgets off that can be found when swiping to the left.
[^2]: The background tabs change to the front tab’s color, so an ESPN tab that changes the bar to red when at the front recedes into blackness if you visit the *Washington Post*.
