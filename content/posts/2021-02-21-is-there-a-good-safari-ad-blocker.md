---
author: Jared
categories:
- Tinkering
date: "2021-02-21T11:54:00Z"
guid: https://eberlemain.nfshost.com/?p=199
id: 199
tags:
- Nerd Stuff
title: Is There a Good Safari Ad Blocker?
url: /is-there-a-good-safari-ad-blocker/
---
<!-- wp:heading -->
<h2>What's the Point?</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>For a while I've bounced around between ad blockers and wanted to finally have some idea about how they compared to one another, so I decided to compare how they stacked up when I opened various websites. What's below is a non-extensive test of the ad blockers.</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2>What's compared</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>I didn't set out to answer which ad blocker on MacOS/iOS is the best because I don't really care. What I was concerned about was which one I've used is the best. I assume I missed some, maybe even a good one, but what's below is not meant to be all of them.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Wipr:</strong> This is really just a wrapper for EasyList, EasyPrivacy, and a number of language-specific lists. It's only option is to auto-refresh the lists. Because of the number of rules it uses three extensions in Safari. Costs $1.99</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Magic Lasso</strong>: The newest one I tried out. Like Wipr, it's a managed app, you can select to allow a community whitelist (websites many people have whitelisted) and select an option for "battery boost," which promises to block problematic javascript and other resources that could drain the battery. App is a $29.99 yearly subscription.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Ka-Block:</strong> Ka-Block is the simplest app here, it uses a hard-coded list, nothing more. Free. I paired it with Hush, a cookie notice blocker and one that is similarly hard-coded and free.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>1Blocker:</strong> One of the first ad blockers I used when Apple released the content blocker function. It has a number of options to add custom rules or turn off blocking for certain filters. Various tiers from free to lifetime subscription.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Adguard for Safari:</strong> Here I'm testing the Adguard for Safari that is a free content blocker instead of the paid Adguard for Mac that essentially works as a proxy for your entire system. I find Adguard for Mac a little too much, especially as I use DNS filtering already, so I'm not super concerned with stuff outside safari. Here I've tested two options, Adguard's default settings (which only enables their ad and tracker blocking lists) and my preferred setup (I add in Fanboy's Enhanced Tracking, and some annoyance filter lists)</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2>Why Not Use Firefox?</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Well, I do. But I've always been annoyed with Firefox as my default browser. For one, it looks decidedly out of place on a Mac, where the default theme has a black bar at the top. I can set it to use either light or dark themes but it does not follow the system theme and if I set it to either light or dark that carries over through Firefox Sync and then makes the browser look out of place on my Linux box. Safari also has the (inherent) benefit of integration with the OS and iCloud tabs for easy access between devices. I also tried using Firefox on iOS (trust me I was happy to see the option to set default browsers come to iOS) but it's clunkier than Safari and just a wrapper for Webkit given Apple's restrictions.</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2>Why these websites</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>I picked five websites based on their history of resource use, ads, and other things I'd want blocked. If you're interested in testing an ad blocker, the best option truly is a newspaper website, especially one in a medium-sized city, because they're loaded with junk.</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2>The Results</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Again, this isn't scientific and I didn't do averages. I loaded each page in a private window with cleared caches. That's it. If you want science, I'm sure someone else has the results. I'm mostly interested in how many domains connect and the resources transferred, but I've included total time load as well. Winners are in bold.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>The Verge</h3>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>Wipr: <strong>10 domains</strong> / 41 resources / 2.59mb total / 1.51 transferred / 2.11s</li><li>Magic Lasso: 17 domains / 53 resources / 3.68mb / 1.8mb / 1.86s</li><li>Ka-Block: 15 domains / 41 resources / 3.68mb / 1.80mb / 1.58s</li><li>1Blocker: 15 domains / 51 resources / 3.74mb / 1.85mb / 1.82s</li><li>Adguard (Default): 15 domains / 47 resources / 2.64mb / 1.51mb / 1.72s</li><li>Adguard (Preferred): 11 domains / <strong>33 resources</strong> / <strong>2.52mb</strong> / <strong>1.24mb</strong> / <strong>967ms</strong></li></ul>
<!-- /wp:list -->

<!-- wp:paragraph -->
<p>Adguard with additional filter lists won all of them easily except for domains, and a re-run of Wipr returned the same results.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>The Oklahoman</h3>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>Wipr: 29 domains / <strong>90 resources</strong> / <strong>3.65mb total</strong> / <strong>1.95mb transferred</strong> / 5.27s</li><li>Magic Lasso: 41 domains / 105 resources / 6.03mb total / 2.36mb transferred / 5.40s</li><li>Ka-Block: 36 domains / 100 resources / 6.16mb total / 2.47 mb transferred / <strong>4.11s</strong></li><li>1Blocker: 33 domains / 103 resources / 4.88mb total / 2.44mb transferred / 4.86s</li><li>Adguard (Default): 34 domains / 106 resources / 6.34 mb total / 2.69 mb transferred / 4.86s</li><li>Adguard (Preferred): <strong>27 domains</strong> / 93 resources / 3.81mb total / 2.21mb transferred / 5.85s</li></ul>
<!-- /wp:list -->

<!-- wp:paragraph -->
<p>Wipr won three categories, Adguard blocked more domains, and Ka-Block was the quickest loading.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>ESPN</h3>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>Wipr: <strong>34 domains</strong> / <strong>300 resources</strong> / <strong>19.8mb</strong> / <strong>2.70mb</strong> / <strong>9.14s</strong></li><li>Magic Lasso: 39 domains / 321 resources / 22.2mb / 10.8mb / 10.92s</li><li>Ka-Block: 37 domains / 312 resources / 22.3mb / 10.6mb / 10.82s</li><li>1Blocker: 39 domains / 333 resources / 22.0mb / 10.6mb / 13.28s</li><li>Adguard (Default): 36 domains / 326 resources / 22 mb / 10.8mb / 9.60s</li><li>Adguard (Preferred): 35 domains / 321 resources / 21.7mb / 10.8mb / 11.47s</li></ul>
<!-- /wp:list -->

<!-- wp:paragraph -->
<p>ESPN was the worst website in terms of resources and Wipr handled it the best in all categories.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>CNN</h3>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>Wipr: <strong>12 domains</strong> / 68 resources / 6.02mb / <strong>1.88mb</strong> / 4.44s</li><li>Magic Lasso: 31 domains / 99 resources / 7.69mb / 2.28mb / 4.30s</li><li>Ka-Block: 26 resources / 97 resources / 7.40mb / 2.25mb / 5.07s</li><li>1Blocker: 25 domains / 84 resources / 6.78mb / 2.08mb / 7.53s</li><li>Adguard (Default): 16 domains / 75 resources / 6.56 mb / 2 mb / 4.36s</li><li>Adguard (Preferred): 14 domains / <strong>65 resources</strong> / <strong>6.00mb</strong> / 1.89mb / <strong>3.94s</strong></li></ul>
<!-- /wp:list -->

<!-- wp:paragraph -->
<p>Wipr and Adguard with additional filters were almost identical, except Wipr blocked two more domains and Adguard loaded quicker.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>The Pirate Bay</h3>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>Wipr: 4 domains / 18 resources / 237.3 kb / <strong>38.7 kb</strong> / 3.59s</li><li>Magic Lasso: 6 domains / 19 resources / 233.7kb / 175.8 kb / 1.79s Ads</li><li>Ka-Block: 8 domains / 23 resources / 237.4 kb / 3.06 kb / <strong>1.32s</strong> Ads</li><li>1Blocker: 5 domains / 14 resources / <strong>184.2kb</strong> / 157.9kb / 1.64s JS blocked</li><li>Adguard (Default): 4 domains / 19 resources / 238.1kb / 181 kb / 1.77s</li><li>Adguard (Preferred): <strong>3 domains</strong> / <strong>12 resources</strong> / <strong>184.2KB</strong> / 157.9 KB / 1.52s JS Blocked</li></ul>
<!-- /wp:list -->

<!-- wp:paragraph -->
<p>I picked a random torrent page on the Pirate Bay given their heavy use of ads and abusive scripts. Both 1Blocker and Adguard with extra filters blocked the main javascript and wouldn't fully render the page. Both Ka-Block and Magic Lasso displayed ads.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>Total Wins</h3>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>Wipr: 12</li><li>Magic Lasso: 0</li><li>Ka-Block: 2</li><li>1Blocker: 1 (with the caveat that it failed to render the page)</li><li>Adguard (Default): 0</li><li>Adguard (Preferred): 11</li></ul>
<!-- /wp:list -->

<!-- wp:heading -->
<h2>Thoughts</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Wipr and Adguard with additional filters were by far the best options. Magic Lasso and the default Adguard didn't secure any wins, and 1Blocker's only victory was on a page it didn't fully render. Ka-Block, for a hard-coded list, performed well compared to something like Magic Lasso given the cost difference.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Given the similarity between Wipr and Adguard with additional filters, it's worth considering that the two have very different resource usage. Both run in the background to refresh, yet Wipr uses around 20-25mb of RAM while Adguard usually sits over 200mb of RAM. In the age of cheaper RAM, the usage isn't a huge deal, but it's noticeable, especially when I'm using an older computer that has less RAM to spare. Adguard's resource use is my biggest source of frustration with the app, and the reason I've sought out alternatives.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>The last thing I will note that stuck out to me is that Adguard's default filters are based on EasyList, yet they seem to have performed worse than Wipr. Wipr has other language filters, a cookie notice filter, and the ad block warning removal list, but many people are not necessarily going to spend a ton of time turning on extra filters in Adguard.</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2>End Result</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>I'm using Wipr, it achieves the best results with the leasst resource usage. You, random internet person who found your way here, should use whatever you want to use.</p>
<!-- /wp:paragraph -->