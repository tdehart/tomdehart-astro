---
title: 'Wildstar'
pubDate: 2022-07-01
description: 'This is the first post of my new Astro blog.'
author: 'Tom DeHart'
image:
    url: 'https://docs.astro.build/assets/full-logo-light.png'
    alt: 'The full Astro logo.'
tags: ["astro", "blogging", "learning in public"]
---
I've always loved tinkering with the user interface whenever a game allows it. I remember modifying ini files in [Tribes](http://en.wikipedia.org/wiki/Tribes_%28series%29) to move around the health bars so that they were easier to see, and I would toy with addons for hours in [World of Warcraft](http://en.wikipedia.org/wiki/World_of_Warcraft) trying to make the perfect interface. Lately I've been playing [Wildstar](http://en.wikipedia.org/wiki/WildStar_%28video_game%29), a new MMO that provides a powerful API for making addons. In fact, the stock interface was developed entirely with the public API so an aspiring addon developer can crack open any element of the in-game interface and poke around (which is important since there's no documentation yet). The Wildstar developers call this [peer-level functionality](https://forums.wildstar-online.com/forums/index.php?/topic/55410-addons-that-display-enemy-units/?p=595084) and it has allowed for a lot of potentially abusive addons like one that [cheats for you](http://www.curse.com/ws-addons/wildstar/220323-cheatsimon) or one that [shows the location of all nearby enemy players](http://www.curse.com/ws-addons/wildstar/220097-thezone).

<!-- ![Wildstar API.png](wildstar-api.png) -->

Unfortunately the Wildstar UI has a lot bugs. In fact, there are [dozens of addons](http://www.curse.com/search/ws-addons?game-slug=wildstar&search=fix) dedicated to just fixing one small thing with the stock interface. I discovered one of these bugs during a beta test — the player's selected mount wouldn't save in between sessions. I spent a few hours learning [Lua](http://www.lua.org/), the programming language used in Wildstar's addons, and implemented a quick hack to solve the problem. I shared it with my group of friends and uploaded it to [Curse](http://www.curse.com/ws-addons/wildstar/220412-defaultmount) where it was downloaded thousands of times. It was eventually fixed in the default UI but I was hooked at this point and wanted to make something more ambitious.

In Wildstar there are "rare" creatures that drop special items or satisfy some sort of in-game achievement when killed. The problem, of course, is finding these creatures in the vast game world. I dug through the API and found that unit information is constantly sent to the game client every few frames. By cross-referencing incoming unit names with those found in the [game achievements](http://wildstar.gamepedia.com/Kill_achievements) I was able to write an addon that detects nearby rares and, thus, [RareTracker](http://www.curse.com/ws-addons/wildstar/220585-raretracker) was born.

<!-- ![RareTracker](raretracker.png) -->

RareTracker ended up being my most popular addon with over 150,000 downloads as of writing this post. I don't work on it much anymore but I spent as much time developing RareTracker and other addons as I did playing the game itself. Though it was sometimes a lot of effort to provide support and grant feature requests, it was very rewarding to work on something that you personally find useful while also providing it to others. Not to mention it was a great opportunity to learn a new language!
