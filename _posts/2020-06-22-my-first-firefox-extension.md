---
layout: post
title: my first firefox extension - tab2hyperlink
---
I don't even remember when I was started to use [Firefox](https://www.mozilla.org/en-US/firefox/new/) as my default web browser. I liked it because it's open source and easily configurable according to my privacy needs. today's internet world is build on tracking and analysing tools which I prefer to leave myself out of it. This concerns can be a topic of another post but you can check [prism-break](https://prism-break.org/en/) for further details. today's topic is my first Firefox extension: tab2hyperlinklist. 

why I coded a firefox browser? as some you already know I'm a kindle lover. thanks to amazon [send2kindle](https://www.amazon.com/gp/sendtokindle/) I'm reading almost every article on my feed from kindle. I'm putting too much effort to find valuable contents for me each week. basically, I'm using [Feedly](https://feedly.com/) to subscribe RSS feeds, using good old email subscription to gather news from both paid or free qualified sources like [BBC](http://pages.emails.bbc.com/subscribe/), [HBR Turkey](https://hbrturkiye.com/), [APISecuritIO](https://apisecurity.io/) and lastly using my simple [script]((https://github.com/cagta/gather-my-news)) to gather weekly news from varios sources. thanks to [dev.to](https://dev.to) I have to update the last one since they do not want bots. while reading all of these articles I'm using clippings function to analyze all of those and if it seems interesting enough to me I'm sharing them with you on the homepage of this blog.

so I have a bookmark directory which is called "blog" to collect all of the valuable resources for sharing with you. even most of them came from kindle sometimes I'm adding stuff from custom resources like youtube etc. at the end of the week I have to open each link from this directory and convert them to something like this:

```html
     <li><span>22 June 2020</span> &raquo; <a href="https://duckduckgo.com/">DuckDuckGo</a></li>
```

so I can share each item with you. these days, it started to seems like a nightmare to me after gathering bunch of stuff I have to put one more manual boring step to make them ready to publish. I decided to write an extension to automate it. what I though is since I'm opening those links for further analysis after gathering clippings from my kindle, I could use that as a start point. 

first I read this very helpful and simple [article](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/Your_first_WebExtension) to understand the structure of the firefox extension. after that I though I can use [Tabs Api](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/API/tabs) to get my needs which is the url of the open tabs and their title. while structuring it I noticed that I have to pick a logo to publish my tiny extension. thanks to [CC License](https://creativecommons.org/licenses/) and the creator of the icon, I pick a little [armchair](www.iconarchive.com/show/free-flat-sample-icons-by-thesquid.ink/armchair-icon.html) which has a strong connection with my armchair fetish =) I love reading stuffs on that. after that I build this tiny little [thing](https://github.com/cagta/tab2hyperlink) which I hope it will make difference for me.

if you want to install that you can check it from [here](https://addons.mozilla.org/en-US/firefox/addon/tab2hyperlinklist/?src=search).