---
title: My experience with Iceshrimp.JS
date: 2024-11-02
last-modified-at: 2024-11-02
tags:
  - social media
  - fediverse
  - ramblings
---

Earlier this year - technically late last year into early this year, I was trialing the fediverse software known as [Iceshrimp](https://iceshrimp.dev/iceshrimp/iceshrimp), lovingly marketed as "YAMF - Yet Another Misskey Fork", because it is (there's a joke that there's new Misskey forks every week). They're actually in the middle of re-writing Iceshrimp to use dotNET instead of Javascript, which will hopefully boost performance down the line. Though, Iceshrimp dotNET was nowhere near "production" stable when I tried it, but I want to give it a go once it gets more polished.

## What I loved about it

{% figure "/assets/images/stickers/HeartSenil.png", "Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

I know people rag on Misskey being bloated, and yeah there's definitely a ton of features I didn't care for, or felt were too similar to each other to make it clear what each was used for - let alone some features don't even *federate* outside of the server, and this was just for me so they were 100% pointless. But Iceshrimp has a *lot* of nice quality-of-life features that I made use of.

### The drive system

Instead of uploading images, videos, audio, etc. every single time you share something - say, you share furry stickers now and then because they're fun and personalized reaction images in a way - everything gets uploaded to a user drive that you have full access to, and you share files via that system instead. I mostly appreciated this for alt-text purposes, since I no longer had to remember to add alt-text every single time I wanted to use a sticker, and could make sure that stuff was captioned in similar ways for consistency. Before I pulled that VPS offline (finally), I would regularly refer back to the files in Iceshrimp whenever I uploaded a sticker.

*(aside: I've literally created a file in the source for this site that solely acts as a way to track the captions for the stickers I use, so that way I can keep them consistent post-to-post and not have to dig through blog posts to find where I used one.)*

I wish I could embed alt-text into image, video, etc. metadata so that way I could upload something anywhere and it'd always have the alt-text set up on the service itself, instead of me having to remember every time how to caption it.

Another thing I like about the drive system? It makes sizing S3 buckets for user-uploaded media straightforward. You can expect to pay for, at most, roughly some amount of money per amount of users at maximum - assuming everyone's drives are totally filled up. Of course, you'll probably never hit that amount, but it's a convenient way to budget storage space and whatnot. When I was looking as using DigitalOcean Spaces, and a 5GB drive size, that comes out to about fifty users per 250GB slice Spaces offers - a neat $5 a month, outbound traffic partly included.

### The bubble timeline

This might be something Mastodon, Pleroma, Akkoma, etc. support, but I know for fact Iceshrimp (and Sharkey, maybe other Misskey forks too) have what's called the "bubble" timeline. This is like the full federated timeline, but only to specific instances that the admins deem "worth" putting into a special timeline. I think this is SUPER handy when it comes to an instance that federates very broadly - giving users a lil selection of known safe instances is a nice touch.

I think it's a clever way to shrink down the mess that would be the firehose federated timeline into a normal hose of curated instances.

### Baked-in translation hookups

Being able to read posts made by people speaking in their native tongue is, to me, important. No translation service is perfect, but it's very nice to at least be able to see what's being talked about. Iceshrimp includs support for two translation services that link up *directly* to Iceshrimp (unlike Bluesky right now, which just shoves you to a Google Translate webpage) - LibreTranslate and DeepL. [LibreTranslate](https://libretranslate.com/) is open source under GNU A-GPL 3.0, and - importantly to me - *can be self-hosted*, which means no paying API costs to some other company, or figuring out some way to bypass the costs. [DeepL](https://www.deepl.com) is commercial and costs money once you go beyond 500,000 characters a month, but it has better language support, and translation isn't dependent on whatever runs your self-hosted setup working, too.

{% figure "/assets/images/stickers/ConfettiSenil.png", "Senil happily tossing confetti in the air. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

Ultimately, though, I just appreciated being able to hit a button and see a post translated from one language into mine *mostly* intact, given the inherent limits of machine translation. Plus, it pretty much always worked compared to X's Google Translate API, which would occasionaly go "nope, can't translate this!" even though it's CLEARLY not in English - and I imagine that happened for folks who speak anything but English and tried to translate from English, too. Mastodon currently only supports DeepL - which is better than *no translation option at all* - but I don't know how many instances bother with hooking it up.

And since DeepL has the whole "you might have to pay at some point" risk for instance admins and operators, I wouldn't be surprised if the lack of baked-in DeepL translation continues.

### Quote posts AND reactions!

Quote posts are a sticking point on the fediverse, for a variety of reasons, but chief among them is that quote posts could enable harassment and targeting of users by enabling folks to easily dunk on The Main Character Of Today. Folks can still do this, though, by just copying a link and pasting it into their post, which (in my eyes) is actually *worse* because it means you have no way of knowing how folks on other instances are responding to you. Potentially making it harder to retroactively protect a user from getting harassed because people are coordinating on a separate instance.

But a built-in quote system, *to me*, is perfect. Both because "quoting posts is part of making something that Feels Like Twitter but Fediverse", but also because it makes it easier to respond to a post in a tangential manner. I've done this a few times with my fake quotes that link back to the original post, but having a "native" solution makes it much easier to work with. Also, folks will quote posts with a content warning if the original post doesn't have one that they think it should have, and "make it easy to do this process" makes it easier for folks to do that. Iceshrimp - really, most fediverse software EXCEPT for Mastodon - support quote posts in some form or another.

Reactions are just fun because they're a fun way to respond to posts - instead of just liking something, you can send a reaction that might better convey your response, instead of replying with a single emoji. They still show up *as* likes/favorites on your profile, but maybe it's a cute little fox holding a heart instead of a basic red heart or yellow star. Yeah, this makes posts subject to Discord Reaction Spam, but I personally think it's endearing in its own right.

{% figure "/assets/images/stickers/HowdySenil.png", "Senil pointing towards the viewier, winking. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

Imagine getting to spell out "KUNG POW PENIS" on someone's post because of some bullshit they said.

### A nicer default web UI/UX

Something that base Mastodon struggles with, in my opinion, is a web experience that most folks might enjoy. The mobile phone UI is atrocious - [go to my Mastodon profile on your phone yourself](https://furry.engineer/@senil888) - what with the column on the right eating up precious horizontal real estate, and the desktop web UI leaves something to be desired personally. Everything is handled via the text box on the left of the screen, meaning replies can get awkward to manage and set up.

Meanwhile, Iceshrimp (Misskey in general, but again I used Iceshrimp) has a nice UI that translates well across desktop, tablet, and mobile. It *feels* like it belongs on all fronts, and that it was designed to fit those environments as best as possible - I used the mobile website pinned to my home screen the entire time. It's not perfect, mind you - Iceshrimp's UI on desktop is REALLY spread out, when I'd appreciate a more central layout that's a bit narrower, something that Sharkey (a different Misskey fork) does have. I got used to it over time, but it was something I'd have preferred out of the box.

{% figure "/assets/images/stickers/ConfusedSenil.png", "Senil dazed and drooling, with a loading icon above him. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

The web UI is also customizable - you can use your choice of themes on the server, find someone else's to use yourself, or create your own color palette if you so desire. It also respects whatever your browser is set to regarding light or dark mode, so it'll swap between those whenever your computer says so. The right side bar? Can be set to show recent notifications, a small posting form if you want, a *clock* or calendar, or nothing at all! It's a small touch - I personally set it up to show me server performance statistics, so I could watch how things ran in real-time.

The VPS was total overkill for a single-user instance federated to whoever I followed, and the [infosec.exchange relay](https://relay.infosec.exchange/).

### Post importing!

This was something carried over from its original base, being the now-dead Firefish (which, yes, was another Misskey fork that a lot of Misskey forks forked from, it's confusing). Unfortunately, that post import tool hadn't gotten necessary love and a security flaw was found where it didn't really respect certain privacy settings on Mastodon posts, so the Iceshrimp team totally disabled it. For good reason, especially given that it wasn't touched since it was first added in Firefish.

Iceshrimp dotNET is supposedly bringing post importing back - which I hella appreciate. Especially since you could even import a Twitter archive. Something I'd love to see dotNET do that Iceshrimp JS doesn't is to *not re-upload media from links.* This was something I noticed when I imported my Twitter archive into Sharkey - which had the same mostly untouched Firefish import tool - and it straight-up uploaded the media of **every single retweet** I ever made.

For hopefully obvious legal and copyright reasons, that's Not Good, and I'd rather posts with media either link back to the original somehow, or use a link to the image on Twitter (or wherever else)'s servers. Not perfect, and this is assuming that's realistic to implement, but it'd make the post import feature a 10/10 for users, and an 8/10 for instance admins. Much less junk uploaded to a user's drive that they legally shouldn't!

## What I didn't really like

{% figure "/assets/images/stickers/AngrySenil.png", "Senil cracking his knuckles with flames behind him. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

So, Misskey and co. are still bloated, and there were a variety of features that Iceshrimp JS has that other software doesn't have (and that Iceshrimp dotNET won't, either). Fortunately, none of these are super major and are easy enough to ignore.

### The god-damn chat system

For SOME REASON, the Misskey developers have a *totally separate* chat system that exists outside of the "normal" direct messaging system, which is basically a normal post that only goes to people you mention (with the caveat that mentioning another user also reveals every previous post). Chats on Misskey can *kind of* work with DMs, but stuff federates weirdly and just doesn't cooperate all that well. Fortunately, Iceshrimp dotNET is getting rid of the separate system while working on a UI similar to it that uses normal direct messaging like everything else does.

I briefly toyed with the chat system. I don't think it's good. Just use DM's like everyone else, or message on a different platform. Custom emoji's didn't even federate between two Misskey-based instances.

### Clips? Channels? Antennas?

I really have no idea what clips or channels are meant for - and either way, they don't really federate outside of the server well (if at all), so they're really pointless for small instances. Antennas, though, are meant to be Iceshrimp's customizable version of following tags, a staple across platforms. They're... annoying to configure, though. And by annoying, I mean really annoying.

It's been a while since I've touched Iceshrimp, but I remember spending a while looking at documentation trying to figure out how to just follow posts with a "#FurryArt" tag. I eventually got it to work, but it came with a flaw of its own - antennas show posts *in the order it finds them*, NOT in reverse chronological order. A post the antenna finds might be five days old that it just stumbled across, followed by a two day old post right below it. It is a more customizable system than just following tags, since you could also filter *out* words and phrases too - say, follow "#FurryArt" but don't show anything also tagged "#NSFW", or something of that nature.

It's a very expansive system that I appreciated, but it felt way too clunky and fairly unintuitive. Posts showing up whenever they arrived, and not displayed in the same reverse chronological as the main timelines, was the sad icing on top for me. If antennae were either a separate timeline entirely, *or* displayed posts reverse chronological instead of "whenever they arrive", I'd tolerate their clunkiness more, purely because it's a much more expansive system than basic tag following.

{% figure "/assets/images/stickers/ScaredSenil.png", "Senil with his hands on his head, mouth wide open in fear. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

### Iceshrimp doesn't have manual account approval

Something a lot of fediverse software supports is registration with manual approval - anyone can technically sign up, but you won't actually be let in unless a moderator OKs it. This is a pretty easy anti-bot system, since you're not [relying on a CAPTCHA that can easily make your service less accessible](https://www.boia.org/blog/how-to-make-captcha-accessible-to-everyone) and thus harder to sign up for with open registration - plus, a CAPTCHA system doesn't stop real people from signing up and abusing your server. Iceshrimp *does* have an invite system, but it's based on invite codes that you have to punch in, instead of an invite link you can just click and boom, you're granted access because you're (presumably) trusted.

This is something Iceshrimp dotNET is going to be adding in due time, but it was a turnoff for me in terms of running something publicly. I don't want to force people to deal with the kinda clunky invite code system, but I also don't want to leave the server wide-open and ripe for abuse by trolls. Some other Misskey forks - Sharkey being the one I toyed with very, very briefly - do have registration with approval. That was honestly a major factor in me wanting to use that for multi-user hosting - despite me overall liking Iceshrimp more.

### The drive system...

**"Wait, didn't you say you really liked it?"**

Yes, I did. And I do like it! But it does present some flaws that I can't ignore. Chief among which is "what is going to prevent users from treating this like a cloud drive?" - capacity is easily capped, but outbound traffic isn't free if you're using an S3 bucket for file storage. Of course, it's easy to just look at who is using a ton of storage and go "hey, please tell me you aren't abusing this." Users with admin access *can* view the contents of everyone's drives - something that I would ONLY ever want to do if I absolutely believe a user is abusing the drive system, or to. You know. Delete copyright or illegal materials hosted there.

There's also the matter of juggling how much space to give people, how big to let uploads be, so on and so forth. I've crunched some numbers and I think a realistic number that most folks won't hit - especially with server-side image and video compression - is around five gigabytes. More than enough space for photos and selfies, short video clips, etc. Iceshrimp isn't meant to be a gallery site like Pixelfed is, and I personally find striking that balance to be hard. But that's just, like, my opinion.

While I said the drive system is great for budgeting the theoretical maximum S3 storage might cost, it might make it harder to change that down the line. I have no idea what happens if you try to shrink the per-user drive allowance while some users have exceeded the new, smaller limits. I don't think I'd want to find out. Growing is is clearly no problem, but it might be easy to give everyone more storage than really needed, and then have to clamp down on storage as more users join in order to keep storage costs lower. I might just be stupid in assuming that, though.

{% figure "/assets/images/stickers/DrainedSenil.png", "Senil lying face-down on the ground, with a low battery symbol above him. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

I don't think the drive system is remotely bad - I think it's a very good idea, and a roundabout way to estimate worst-case costs for S3 object storage, should you pay for that. It's just, well, "A Drive", which means you now need to deal with everything "A Drive" entails. And I *really* don't like that admins can just zoom in and see the contents of someone's drive for privacy reasons, whether it's been posted anywhere (even in a private DM!), but I *do* get it from an admin view, especially when it comes to users hosting blatantly illegal content that can get an instance shut down. Makes it easier to clean them up, maybe?

## So... yeah

I really enjoyed my time with Iceshrimp - I'd probably still use it if it wasn't for the frustration that is "federating a single user instance". I love the software, despite some of its quirks, and I'm really looking forward to what Iceshrimp dotNET is going to bring to the table as it gets more and more polished.

In the meantime, I'll just chill out on Mastodon and deal with the "meh" in my eyes. I'll move over at sime point, maybe self-host again on a cheaper VPS if I don't run it on my own box(es).

{% figure "/assets/images/stickers/SleepySenil.png", "Senil sprawled on his back, sleeping. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}