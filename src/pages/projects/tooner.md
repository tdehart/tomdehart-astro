---
layout: '../../layouts/MarkdownProjectLayout.astro'
title: 'Tooner'
pubDate: 2022-07-01
description: 'This is the first post of my new Astro blog.'
author: 'Tom DeHart'
image:
    url: 'https://docs.astro.build/assets/full-logo-light.png'
    alt: 'The full Astro logo.'
tags: ["astro", "blogging", "learning in public"]
---
<!-- ![Tooner](tooner.png) -->

Shadowbane was a popular MMORPG that released in 2003 and was known for its hardcore gameplay, city sieging, and large-scale battles. Unfortunately the game was plagued with bugs and the client was incredibly unstable. The launch was a failure even by 2003 standards but it did manage to last 6 years until the servers were shut down indefinitely. Despite Shadowbane's lack of widespread adoption it did have a zealous fanbase that played the game until the very last day. As is often the case with older MMORPGs, emulators started to spring up in an attempt to replace what was lost. Low budget operations like [Shadowbane Emulator](http://shadowbaneemulator.com/) and [Magicbane](http://magicbane.com/) are small by today's standards but still have active communities that keep the game alive. When the official servers for MMOs die, the game lives on entirely through its community and recreating an MMO with nothing but a reverse-engineered client is an amazing feat, especially when the developers don't even accept donations.

Shadowbane has a fairly complex character system where a few misplaced stat points can ruin your build forever. Optimizing your build is important in highly competitive games so people often plan their characters well before they're made, making sure that every single stat pooint is distributed correctly. There are many ways to build a character: twelve races, around twenty classes, and over a hundred of character augmentations called "runes". Everything can be mixed and matched which leads to thousands of different combinations.

It's always fun building something to solve one of your own problems (and it's a nice bonus giving back to the community) so I built [Tooner](http://tooner.herokuapp.com/), a character builder for Shadowbane meant for fine _tuning_ your [toons](http://gaming.stackexchange.com/questions/77192/what-is-the-source-for-calling-your-characters-toons). Tooner was built with the [MEAN stack](http://mean.io/#!/) and Bootstrap for HTML/CSS. Only allowing valid Shadowbane characters to be built was important to the app and maintaining validation with every user choice was so simple Angular's data binding. Instant feedback was necessary when, for example, certain character augmentations were no longer selectable based on previous choices. DOM manipulation with directives made this incredibly easy. I can't recommend Angular enough when it comes to building an app like this!
