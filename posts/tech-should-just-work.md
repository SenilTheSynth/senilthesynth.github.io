---
title: Some thoughts on "software for non-techies"
date: 2025-01-12
last-modified-at: 2025-01-12
tags:
  - ramblings
  - tech
  - foss
---

This blog post is a refined version of my thread from booping.synth.download, regarding [this specific post that I stumbled across](https://retro.social/@ifixcoinops/113790985784272965), and wanted to expand on it with my own thoughts in agreement with OP.

## Normal People != Tech Nerds

{% figure "/assets/images/stickers/ScaredSenil.png", "Senil with his hands on his head, mouth wide open in fear. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

If you want your software to be used by Normal People (and you aren't in an industry environment where slightly more specialized things are going to be training anyways), you gotta approach them on Normal Person Terms. The biggest one being "does this new thing still do what I needed the original for" paired with "can I just hit install and get going with no fuss." Very few Normal People sign up for a social network because privacy or some other abstract reason. They sign up because their friends are there and they think it'll be a good community. They stick around if the culture is good and the system is Intuitive. 

They do not care about much otherwise. Which is ok! I'm the same way with certain things in my life - I'm willing to fight some to make shit work how I want it to, instead of how (insert random company here) wants it to, but 87% of the time I just want shit to work. 

Sure, I could use Linux on my desktop when I set it up again, but I want to use CAD tools that are kinda the industry standard here, which means AutoDesk, which means no Linux. There are hacky ways to make it work, but I'd be fighting it enough as is. I don't need getting the thing to run to be part of it. 

Y'know why most Normal People don't use Signal or Matrix or whatever? Because a) their friends and family probably aren't on it, b) that is Yet Another Place to keep tabs on, and c) *it doesn't really do anything else for them.* Assuming it even works half the time, too (*cough* matrix *cough*)

{% figure "/assets/images/stickers/AngrySenil.png", "Senil cracking his knuckles with flames behind him. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

## Stop assuming shit y'all

Approach folks where they're at. You aren't going to get people who just want to talk to their friends to sign up for a social platform that talks way too much about the backend and not enough about what it does and its features and how nice it is to use and find friends and communities and whatnot. They don't care about federation, they just want to hang out. 

I'm so annoyed by anyone who assumes that Most People just want their tech to work and not fight it. It's part of why any local self hosting (for others) is going on micro boxes that sit behind another one on a totally different physical network that's regulated by the larger box. Sure I could fuck around with vlans and ports and access restriction and shit, but it's way easier for me to just go "this is the literal only thing that's physically part of the rest of my network, it's the only thing that gets to talk to the outside world, and it's the thing in charge of handling everything else."

I'd be fighting that box (& the others) enough as-is. I don't need to be juggling shared physical networking stuff to try and keep things otherwise separate and secured. And I'm already technically minded.

I don't care about the backend about a lot of things unless it's a personal project, I'm paid to care about it, or the ADHD kicks in. I just want shit to work & anything that prides itself too much on the backend without talking about the actual experience (let alone "what does that mean for the end user") is an Orange Flag for me.

## I'm like, the wrong person to argue this

Yes this is kind of rich coming from the guy who wants to fuck around and install postmarketOS onto a ChromeOS tablet (an HP Chromebook x2 11 in particular), but the only reason I really care to fuck around with that is a) it sounds interesting, and b) *I don't care about that tablet anyways*. It sits unused, it doesn't do shit 99% of the time these days as is. If I fuck it up, it's not a massive loss on my part.

{% figure "/assets/images/stickers/ConfusedSenil.png", "Senil dazed and drooling, with a loading icon above him. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

#### A lot of folks don't have that ability to fuck around & find out.

There are a lot of things to my tech that I could modify to make it more secure or de-Google things, but I want stuff to just work - yeah I could install GrapheneOS on the Pixel I plan on getting, but if something happens it's on me to troubleshoot instead of getting to pass it off to Google. I know I'm damn well not alone in that aspect, there's a reason that even among technically minded folks that rooting and custom ROM use has gone down (outside of Google making it harder to do and more annoying to use normal things).

Like, I want to set up a nice smart home someday. I don't want shit on WiFi for various reasons (mostly that's more things cluttering up the network), so I'm stuck with using Zigbee, Z-Wave, or Thread as the backend. The only "smart" things I have are three WiFi bulbs from Yeelight (also known as Xiaomi) that I got a while back because they were cheap and they mostly worked. I don't really care if I end up replacing them or delegate them to like, a lamp. However, when it comes to Matter-based smart devices (of all flavors, Matter over WiFi or Matter over Thread), not all ecosystems are the same - which **infuriates** me.

{% figure "/assets/images/stickers/DrainedSenil.png", "Senil lying face-down on the ground, with a low battery symbol above him. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

Apple has relatively expansive support for many Matter devices, and a lot of Matter devices also have extra functions if you use HomeKit too. Google has more limited pool of what works with their Matter system, and the same story applies for Amazon. Samsung's Smartthings supports everything up to Matter 1.3, as does Home Assistant. I don't *particularly* want vendor lock-in, so that leaves me with either Smartthings or Home Assistant.

This involves a lot of backend tech stuff I get the joy of setting up, which I wouldn't have to fight as much if I used Smartthings instead, but I'm personally willing to fight *some* of my future smart-home tech to make things work My Way. Not everyone is, and that's why I wish Apple, Google, and Amazon all had full support for Matter 1.3 devices (and fully support Matter 1.4 once that version establishes itself). If you don't know that Samsung is the only system with full Matter support, you might be left in the dark because something that should allegedly work just fine with your Google might not at all anymore.

The only reason I care to fuck around with Home Assistant for Zigbee and Thread and Matter is that none of those devices are in my home yet. I don't own a single Zigbee or Thread or Matter smart device sensor whatever yet, which means I have zero switching cost involved. If I had a couple of smart plugs, a couple sensors, a lightbulb or two, maybe a wireless remote button... well, that equation changes things because my setup works just fine like that.

{% figure "/assets/images/stickers/SleepySenil.png", "Senil sprawled on his back, sleeping. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

Why throw it all out the window just to put that in my control when it already works? I want to be able to yell at something to turn a light on or off, or have something happen when I leave home, or be able to monitor something from my phone remotely (be it sensor stuff, energy, or a CCTV system). If that shit is in place already... why fuck around trying to "improve" things, leaving me without that system until I get it working again but Differently?

## Switching costs exist, too

I want everyone - of all stripes, but obviously tech nerds right now - to remember that switching costs exist. People get familiar with an ecosystem, and the more familiar they are - and the more they buy into it - the harder it becomes to convince them to try something else. Even if someone has relatively low switching costs in terms of their ecosystem buy-in, are they technically minded enough or whatever to make that change relatively un-supported?

Sorry to use you as an example here, fiance, especially since we just talked about this the other day, but you're a good case study here. I know that the vast majority of their compute needs could be handled by a stable Linux distro that "just works" as much as possible. The only clear exception being games with kernel-level anti-cheat, which is hopefully going away eventually [since even Microsoft has acknowledged that it's insecure](https://www.notebookcheck.net/Microsoft-paves-the-way-for-Linux-gaming-success-with-plan-that-would-kill-kernel-level-anti-cheat.888345.0.html).

{% figure "/assets/images/stickers/HeartSenil.png", "Senil hugging a big pink heart. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

However, even though Windows is, well, Windows, and not particularly enjoyable to use, Windows is what they're extremely familiar with. Even though in theory (and in my months of running Aurora on my laptop as my only computer for months now, in practice) they'd have no problem switching away given that everything they run would work fine on Linux, actually doing that is a hassle in its own right. There's suddenly a whole user interface and experience to get used to, a new set of software paradigms to at least get loosely familiar with, and its own set of quirks to learn as well. All of which would be at best adjacent to Windows, and at worst sizeable departures from what they're familiar with.

This is the case for MANY people out there. They don't care that Linux is free and runs better and is more secure than Windows given, uh, Recall is still a thing. Windows is still *what they know* - and it makes more sense to get Microsoft to make Windows a more enjoyable experience for those who don't, or even CAN'T, move to something else. Think of how much enterprise software is Windows only, or *maybe* Windows and MacOS. You might be able to hack something together to get that software to run on Linux, but now you're fighting both the software as well as the ability to even launch it in the first place.

## Live and let live

{% figure "/assets/images/stickers/HuggingSenil.png", "Senil hugging a generic YCH furry. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

Shockingly few people outside of tech nerds, privacy advocates, and those around them care much about how secure a platform is, or the end-goal of the platform, or stuff like federation when it comes to ActivityPub software. They want something that works for them, and that they're familiar with. As I've seen folks on Fedi say - and a sentiment I agree with - "The year of the Linux Desktop will come when you can go into Best Buy and buy a laptop with Ubuntu on it for $400."

The year that E2EE chats that aren't controlled by scummy corporations like Meta will come when people use it, and it presents as good an experience as what they're already used to. The year that there's even somewhat a return to the old web in structure will come when the onboarding is straightforward, when the software is intuitive, and where things "just work" with each other. People shouldn't need to open up the original post every time just to see all of the replies their instance didn't find. People shouldn't feel threatened to lose their friends every time a defederation happens, or an instance shuts down out of nowhere and they can't actually move shop.

A lot of people want folks to stop using Twitter/X, Facebook, Instagram, and similar. But that won't happen until the alternatives that are *on paper* better, become, well, actually better, with a user base large enough to make people at least want to say hi cause their friends are there too.

{% figure "/assets/images/stickers/SadSenil.png", "Senil curled into a ball, crying. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

Sorry, Friendica, but talking about how secure you are and what federation is like isn't going to sway the average person. That's something only nerds care about or even understand.