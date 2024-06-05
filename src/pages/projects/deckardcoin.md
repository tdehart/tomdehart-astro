---
layout: '../../layouts/MarkdownProjectLayout.astro'
title: 'Deckard Coin'
pubDate: 2022-07-01
description: 'This is the first post of my new Astro blog.'
author: 'Tom DeHart'
image:
    url: 'https://docs.astro.build/assets/full-logo-light.png'
    alt: 'The full Astro logo.'
tags: ["astro", "blogging", "learning in public"]
---
I've held off writing this for 2 years because exploiting online video games is a touchy subject and most gamers have a (justified) hatred towards those who do it. Also it didn't help that the VP of Legal Affairs at Blizzard Entertainment threatened me with a lawsuit if I didn't stop what I was doing. I've always wanted to write about it because I think it's an interesting story and reading [this blog post](http://diablo3story.blogspot.com/2014/07/a-diablo-3-story.html) has finally convinced me to get it out there. So this is a story of making thousands of dollars playing the video game Diablo 3, creating and selling a bot that helped destroy the game's economy, nearly getting into legal trouble, then getting permanently banned from PayPal. This all happened in the span of two months.

First a bit of context: [Diablo](http://bit.ly/1pSLIOm) is an action RPG with a heavy emphasis on player-found items. Items are obtained quite simply by killing computer-generated monsters, and your character's ability to kill harder monsters (which drop better stuff) is almost entirely dependent upon the quality of your gear. The ultimate goal of any Diablo game is to get cool loot and kill harder monsters, then get cooler loot and kill even harder monsters, and so on until you quit. It seems like a fruitless pursuit but the franchise is wildly popular with Diablo 3 having sold more [15 million copies](http://www.ign.com/articles/2014/02/07/diablo-3-surpasses-15-million-sales) since its release.

<p align="center">
  <img src="/images/loot.jpg" class="blog-img"/>
  <span class="caption">Loot drops can trigger a <a href="http://www.psychologyofgames.com/2012/06/the-psychology-of-diablo-iii-loot-part-3-dopamine-binds-on-pickup/">dopamine release</a></span>
</p>

Item-centric games like Diablo almost always have popular virtual economies where saavy players (with a lot of time on their hands) are able to make a quick buck pawning their goods to casual players with disposable income. Everyone wants to have a powerful character and, when items determine the bulk of your strength, the only way to get them is to either spend a lot of time playing, or spend a lot of money. Where there is money to be made you will eventually find entrepeneurs moving in to optimize the delivery of goods to the buyers. As such, virtual currency farming, or [gold farming](http://en.wikipedia.org/wiki/Gold_farming), is estimated to be a [multi-billion dollar](http://www.theguardian.com/world/2011/may/25/china-prisoners-internet-gaming-scam) industry.

Gold farmers ruin the gaming experience in a number of ways and are infamous for spamming chat channels and using in-game messaging systems to mass advertise their services. Even worse, people employed by gold farming companies are [being exploited](http://massively.joystiq.com/2008/10/25/gold-farmers-connected-with-$-38-million-money-laundering-bust/) for cheap labor in order to meet buyer demand of in-game goods. On top of this, these shady companies use social engineering and brute force attacks to hack player accounts. World of Warcraft characters, for example, are commonly worth [hundreds or thousands of dollars](http://www.playerauctions.com/wow-account/) which is [fueling](http://news.cnet.com/No-end-in-sight-to-hacking-of-WoW-accounts/2100-1043_3-6174704.html) the practice of hacking accounts.

<p align="center">
  <img src="/images/spam.png" class="blog-img"/>
  <span class="caption">Every MMO player is familiar with this</span>
</p>

In an effort to stop the arms race against gold farmers and alike, Blizzard decided to legitimize the trade of virtual goods by introducing a [real money auction house](http://us.battle.net/d3/en/blog/6360586/real-money-auction-house-now-available-in-the-americas-6-12-2012) (RMAH) in Diablo 3. Instead of dealing with shady businesses in order to buy in-game currencies, players could now buy directly from others and it was all facilitated by Blizzard. Their intentions were pure but Blizzard later found that the RMAH [undermined Diablo's core gameplay](http://us.battle.net/d3/en/blog/13354139/diablo-iii-auction-house-comes-to-a-close-3-18-2014) which resulted in them shutting it down 2 years later. But not before [people like me](http://venturebeat.com/2014/03/19/meet-the-gamers-who-earned-big-in-the-now-closed-diablo-iii-real-money-auction-house/view-all/) made tens of thousand of dollars in just a couple months.

Game economies has always been a fun pastime for me. I loved collecting [rare items](http://www.uoguide.com/Rare) in Ultima Online, I strived to be the richest auction house "baron" on my World of Warcraft server, and I sat on [d2jsp](http://www.d2jsp.org/) for hours flipping goods in Diablo 2. When Blizzard [announced the RMAH](http://us.blizzard.com/en-us/company/events/diablo3-announcement/#auction:auction-summary) for Diablo 3 I was poring over beta screenshots and hypothesizing about how I could optimize my income. I even started a virtual economy blog (which never took off) with a couple friends as a result of the hype.

When Diablo 3 finally came out we hit the ground running. We started the moment the login servers came up and hit max level in a day. Within a week we had characters optimized for running static [resplendent chests](http://www.diablowiki.net/Resplendent_Chest) and were selling the items on the auction house. Our original goal was just to make enough money to break even with the game's price. When we ended up with around $2,000 USD worth of gold to split between 5 people we were ecstatic! We didn't realize at the time that we were just scratching the surface.

In a Diablo 3 IRC channel that I hung out in someone posted a screenshot of a weeks worth of their auction house transactions. He bought and sold over a hundred items, many netting him tens of millions of gold each. Even with 5 people running our resplendent chest scheme we weren't coming anywhere close to this single person's income. It wasn't hard to figure out from the screenshot that he was simply buying low and selling high – it turned out that the average person was vastly underpricing their items. Once discovering this we pretty much stopped playing the game itself: the new game was the auction house. 

<p align="center">
  <img src="/images/deckard-coin-01.png" class="blog-img"/>
  <span class="caption">Simple: buy low, sell high</span>
</p>

We spent hours tweaking our search criteria and discovering all of the obscure items that people wanted. It wasn't enough to pursue commonly sought after gear like [Blackthorn's Surcoat](http://us.battle.net/d3/en/item/blackthornes-surcoat) or [Andariel's Visage](http://us.battle.net/d3/en/item/andariels-visage). Instead we would look for stuff like underpriced rare rings and amulets that most players didn't even realize yet were highly valuable. We managed huge spreadsheets to track the buy and sell prices of every item that passed through our inventories. Instead of working together as a group like we did before, we kept our search lists and spreadsheets closely guarded. It was mostly so that we didn't tread on each other's markets, but it was also a vicious competition where we bragged about our profits each day.

It didn't take long for us to start using scripting tools like [AutoHotkey](http://www.autohotkey.com/) in an effort to automate the process. In fact, we were pretty late to the party by the time we had our first "bots" up and running. It was not uncommon to get a hit on a good item just to see it disappear before your eyes as some other bot snatched it up before you. The bigger problem was that these scripts were often slow, took over your mouse/keyboard, and required full focus of the game client. Further, these scripting languages were not great for making complex applications. The optimal Diablo 3 gear was a moving target as people pushed their characters into harder difficulties, so extending our scripts to meet new search criteria was an arduous process and tweaking mouse coordinates for every new item. If we wanted to run more than one script at a time we had to set up spare computers, which many of us did. As we expanded our operations we were desperately looking for a new bot that would solve some of these problems.

Our first break was with a bot posted on a Diablo 3 hacking forum that was capable of reading an XML-formatted list as your search criteria. No longer did we have to manually augment X/Y mouse positions and string inputs every time we wanted to search for something new – the bot figured all of that out for you! Unfortunately it still required full focus of the window and it completely took over your mouse and keyboard. Additionally, it depended on the layout of the auction house user interface, so one day when a major patch made significant changes to the UI, the bot broke completely. The author was kind enough to post the source so I poked through the code and learned how it worked. I got a friend to help me repair the [search criteria list](https://github.com/tdehart/DeckardCoin/blob/master/AHBot/SearchQueryFilters.cs#L107-L282) and we were back in business.

After spending that day learning how the bot worked I became motivated to make something better. The author solved a lot of the grunt work, like constructing a lookup table to figure out item/stat restrictions, but there were various shortcomings that I wanted to fix (like multi-client botting). I knew next to nothing about Windows desktop development but my research eventually led me to Windows [PostMessage](http://msdn.microsoft.com/en-us/library/aa923831.aspx), a low-level function that allows two windows to communicate with each other. The official documentation is vague at best but this single function, I soon found out, was the workhorse of many successful gaming bots. I also came across a neat library written for botting that would allow me to replace unreliable pixel detection methods with memory reading routines. The only problem was that these tools were both native to C languages and the bot was in Java. Undeterred, I spent the following week learning C# as I ported over the entire auction house bot. 

Building the bot was a lot of fun even though [my code](https://github.com/tdehart/DeckardCoin) was probably crap. In an effort to beat everyone else to the punch, I worked 16 hour days until it was done. Our failed virtual economy blog didn't need it anymore so I took the name _Deckard Coin_, a play on words of an iconic character in the series named [Deckard Cain](http://diablo.wikia.com/wiki/Deckard_Cain) who was known for his vast knowledge. The [resulting product](https://www.youtube.com/watch?v=H-ZRnsiEpu8) was actually better than I expected. It was lightning fast for something that didn't inject into memory and could hook into any number of clients which was completely unique at the time.

<div class="center-block">
  <iframe class="youtube-vid" src="//www.youtube.com/embed/H-ZRnsiEpu8" frameborder="0" allowfullscreen></iframe>
  <span class="caption">Deckard Coin in action</span>  
</div>

At this point we were raking in the money with our group of botters easily making over fifteen grand a week combined. Our finely tailored search lists grew to include hundreds of different variables and we'd wake up every morning with a new load of valuable items to resell. We were regularly buying new copies of the game to replace banned accounts and to expand our numbers. We purchased disposable prepaid phones just so that we could verify multiple accounts and move higher volumes through the RMAH. It was a huge operation that consumed 12+ hours a day from each of us. After a while it wasn't even fun but we couldn't stop because it was so lucrative. 

By the time I had finished developing the first version of Deckard Coin, we had already started to see a decline in our average daily income. People were quitting the game after the initial rush, gold was inflating due to farmers, and players were becoming smarter about their auction prices. None of us stopped botting but I started to anticipate a point where the effort no longer matched the return. So against advice from several people smarter than me, I decided to start selling Deckard Coin. And it all came crashing down.

Recall that no auction house bot at the time could provide anything close to Deckard Coin. It was a mishmash of poorly coded C# but it blew away everything else that was publicly available at the time. One weekend, I whipped up a simple Rails app with authentication, dropped in Bootstrap, and deployed it to Heroku. I didn't even have auth built into the bot itself but I wanted stay ahead of the competition. That weekend, I started selling it to small gaming communities on IRC. Some were suspicious but early reception was mostly good. I spent the next few days making tweaks to Deckard Coin in preparation for a more public launch.

I started publicly selling the bot on a Tuesday by posting a thread in a popular botting forum. By Friday of the same week I had received a cease and desist from Blizzard Entertainment and was facing dozens of reversed PayPal transactions. The three days between these two events were an absolute frenzy as I managed the distribution of website logins, provided support for confused customers, and attempted to soothe those that doubted the integrity of the bot. I even brought on a new developer and started splitting some of the profits as we worked on new features day and night. I was essentially running my own business and it was fun as hell. It felt like weeks had passed but three days was all it took until Blizzard took notice and told us to close up shop.

On the morning of July 6, 2012 my friend who owned the domain deckardcoin.com received a call from [Rod Rigole](http://members.calbar.ca.gov/fal/Member/Detail/181389), the VP of legal affairs at Blizzard Entertainment. My friend at first thought it was a prank call but it soon became clear that they were not messing around. We were to wipe the existence of Deckard Coin from the internet, or else face severe legal consequences most likely resulting in us being completely bankrupt. Oh, and we were told not to repeat anything he had just told us. In just a few days I had made thousands of dollars selling copies of my software that was a simple unprotected executable. Not only that, but I was having fun developing and supporting a product instead of managing spreadsheets and staring at the auction house. I knew in the back of my mind that it was over but I was in denial and sought advice from other bot developers to see if I could fight back. Their advice confirmed that I was stupid to even think about trying to sell such a thing without any form of legal protection. Undeterred, I went through and started renaming the bot, registered a new domain, and created a new PayPal account. It dawned on me later that night, however, that it wasn't worth the hassle. We were already outed and I didn't want anyone to get into any more trouble. Blizzard has a [proven track record](http://en.wikipedia.org/wiki/MDY_Indus._LLC_v._Blizzard_Entm%27t,_Inc.) with these sorts of things and it was obvious I stood no chance. I deleted my posts, took down the website, and waited to see what happened next.

There's a lot of mistrust in the hacking and botting communities since viruses and scams are common. Read through the [Deckard Coin thread](http://www.ownedcore.com/forums/diablo-3/diablo-3-bots-programs/362192-release-deckard-coin-auction-house-bot.html) to see evidence of this suspicion. When I abruptly deleted the content from my posts and took down the website it was no surprise that I was branded as a scammer and banned from the forums. Within hours, half of my customers had already disputed their PayPal transactions and, without any real claim to their money, I decided to refund anyone that asked. After all, I advertised lifetime support and the bot did require an update with every game patch. A few customers were happy to let me keep their $50 since they had already made thousands of dollars back from the investment. Most of the money, however, was lost. My PayPal accounts were frozen for suspicious activity so I could no longer sell anything on the RMAH. The disputes lasted over a month while I made new PayPal accounts and rode the sinking ship that was the Diablo 3 economy. It wasn't long until PayPal found my fake accounts and froze them too. After a prolonged investigation they decided that I was too much of a risk proceeded to permanently ban me from PayPal despite me granting refunds to everyone.

After my demise newer and better bots sprung up, and the competition was fierce. As gold farmers improved their methods inflation became more of a problem. Legit players simply could not compete and, those that didn't spend real money to buy gold, were muscled out of the economy as botters relisted everything at exorbitant prices. Posts [like these](http://www.reddit.com/r/gaming/comments/vmgg5/diablo_3_is_plummeting_an_active_public_online/c55s06n) epitomized public opinion at the time. Diablo 3 was in shambles and remained that way until the auction house was eventually [shut down](http://us.battle.net/d3/en/blog/10974978/diablo%C2%AE-iii-auction-house-update-9-17-2013) and [trading was disabled](http://imaginarymarkets.com/patch-2-0-1-live-on-diablo-3-gold-no-longer-tradeable-legendaries-and-set-bind-on-accoun).

<p align="center">
  <img src="/images/rmah.jpg" class="blog-img"/>
  <span class="caption">Screenshots like these were commonly passed around in an effort to brag. <a href="http://www.reddit.com/r/Diablo/comments/xqv2r/ive_made_10000_legitimately_from_the_d3_market/">(Source)</a></span>
</p>

Most of us had made around $20,000 from the auction house in just two months, some even more than that. Being a poor student at the time, this was a welcome influx of wealth. While fun and lucrative, I was relieved when I finally quit. It required an obscene amount of time every day to manage spreadsheets, research new items, and tweak search values. I don't miss it. There will always be new games on the horizon that offer the ability to profit from the sale of virtual goods, but I doubt we'll see anything like the Diablo 3 real money auction house again. It was a perfect storm consisting of a hugely popular AAA title, poorly designed game systems, and a painfully misguided attempt to legitimize the gold selling black market. Diablo 3's lead designer Jay Wilson [went down in flames](http://www.cinemablend.com/games/Blizzard-CCO-Defends-Jay-Wilson-Says-They-re-Listening-Diablo-3-Community-51620.html) for these mistakes (and others). Meanwhile his replacement, [Josh Mosqueira](http://www.diablowiki.net/Josh_Mosqueira), has been doing a great job rebuilding it from the ashes and I recommend anyone that quit during the shaky launch to give the game another try. You'll still find plenty of bots, though.