---
title: Gateway to the Fediverse, or have a local community?
date: 2024-12-09
last-modified-at: 2024-12-09
tags:
  - social networks
  - ramblings
---

This post is brought to you by some recent-ish "discourse"? On the fediverse regarding the purpose of instances in the broader fediverse network, in addition to someone's observation as to the shift from an instance being the gateway to a broader network, into the current view of an instance being a local community that *happens* to connect to the broader fediverse.

And I have some Opinions™ on this matter.

{% figure "/assets/images/stickers/ConfusedSenil.png", "Senil dazed and drooling, with a loading icon above him. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

## Gateways to the network

The general understanding of instances on the fediverse is that they're gateways to the broader network, managed by moderators and with people that are chill to be around. In my eyes, this is more or less how the vast majority of instances that widely federate to others operate. Block out the obvious bad actors, but prioritize access (even limited) to the broader network unless there is something serious enough to warrant a full instance suspension.

As a personal view, *this is more or less how it should be*. There's arguments to be made as to what the lines are for limiting or suspending remote instances or users, but those are highly dependent on instance admins and their moderation policies. I have zero thoughts onto where those lines are, outside of "keep the bad actors out and monitor for those who show signs of it." That's pretty much all I have on what those bounds are.

As an aside, *should* I ever self-host a fediverse instance for others, this will more or less be the stance I take. A gateway to the fediverse at large, with a moderation team people already know and trust, since this would be spun off from an existing group that's been on Discord for years now. I'd take the initial precautions - suspending well-known Nazi instances and the like, and avoiding limiting any others until we're more established and have a bit of a reach where limiting a whole instance becomes a question.

{% figure "/assets/images/stickers/HeartSenil.png", "Senil hugging a big pink heart. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

## Local community (to the network)

"Instances as a community" is the other take that was mentioned in the post that inspired my own version of it, and is the one that I personally dislike. I think it's totally fine for an instance to be focused around one aspect, or more targeted towards certain user groups (meow.social being a large furry instance, tech.lgbt being intended for queer techies, mastodon.art being the huge art instance, etc.), however it *can* become a problem when it's community first, gateway second.

The "community first, gateway second" approach is *totally* fine in my eyes - there is absolutely nothing inherently wrong with it. The problem - in my eyes - is when such an instance claims to be a gateway to the network, but is also clearly trying to be its own community. There are some instances that are meant to be this way from the start, suspending a ton of instances from the get-go. This leads to them effectively operating as an allowlist instance, where only select instances are allowed to talk to that one.

There's nothing wrong with it - so long that it's set up that way from the get-go or early on, and hopefully is communicated and advertised as such to members. Instances that initially work via denylists (aka the default behavior for fediverse instances) suddenly trying to change to an allowlist format creates problems.

## Breaking social links

{% figure "/assets/images/stickers/ScaredSenil.png", "Senil with his hands on his head, mouth wide open in fear. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

The major, number one problem when it comes to outright suspending an instance is the matter of severing follows and whatnot between the two. Mutuals on the other instance will suddenly disappear to the aether if the whole instance is suspended, and herein lies the ultimate concern. A major instance defederating from another major instance is bound to break dozens, if not hundreds or even *thousands* of social links between the two, and even if that suspension is reversed, it's very difficult to get those links back.

This was seen firsthand when mastodon.art (dotArt henceforth) was suspending instances for unclear reasons when "The Bad Space" was *the* source of fediverse meta and drama last year - I do not know enough of what all was happening at the time, nor do I have the willpower to find out, so all I will mention is it caused a huge uproar across large swaths of the fediverse, and in my opinion ended up *damaging* the image of fedi as a whole.

{% figure "/assets/images/stickers/AngrySenil.png", "Senil cracking his knuckles with flames behind him. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

The lead admin of dotArt, having close ties to various other instances, started defederating *entire instances* for unclear reasons, on occasion based on the actions of a handful of members or admins during a chaotic and stressful time as everyone is collectively figuring out what the hell is going on, what to make of it, and how to move forward from here. dotArt is a *huge* instance, with roughly 4800 active users as of me making this post (this is nothing compared to the flagship instance, mastodon.social, with a whopping 280000 active users, though).

This, of course, leaves out the many, many users who aren't super active but still post on occasion - especially back in 2023 when the lead admin of dotArt was defederating large instances for the actions of a few.

For hopefully obvious reasons, this meant a lot of artists and creatives who posted on dotArt, who had a long history of working on dotArt, suddenly lost out on tons of potential clients for commissions, project work, freelancing, etc. All because their instance's admin defederated from many instances - the worst part is those who had clients on those suspended instances suddenly lost contact with them if they only communicated via the fediverse, and those clients could never see the artist's works without going to their page manually.

Slight aside: This happening is one of the key faults with the federated structure as a whole - all it takes is one person (or a small handful of people) to cut off instances from the entire network. Be it by mass blocking others for no clear reason, or by giving up because they can't deal with the myriad stressors of being an admin and quickly pulling the plug on their server. This is something that fundamentally can't happen on a much more centralized network, barring gigantic blocklists *claiming* to filter bad actors actually containing a fuck ton of normal people too.

## The fault of gateway-first

{% figure "/assets/images/stickers/DrainedSenil.png", "Senil lying face-down on the ground, with a low battery symbol above him. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

The risk of breaking social links under a "local community first" approach (which could be very trigger-happy with suspensions) doesn't magically mean that a "gateway to the network" approach is perfect and ideal and has no problems whatsoever. This approach has its own flaws. The biggest of which, in my eyes, is that moderation is *extremely* reactive. Because of this priority, any infraction of standards that other instances are held to is harder to evaluate.

Does instance size matter? What about the severity of the infraction? Is it one member or dozens? Is it a moderator or the lead admin doing this? Is that instance even well moderated, or is this just a momentary lapse in mod activity for some reason? All of these factors *and many more* could play a role into making these kinds of decisions. When acting as a "gateway first" instance, initial actions set precedence for the future.

Instances should be held to the same set of standards, after all. It's ridiculous to set one decision early on for one instance, and then months later make a different decision for a different instance that otherwise meets the exact same criteria as the former one. The way to manage this is to keep a somewhat detailed log of actions, in perhaps a "burn book" of sorts, in order to provide easy-to-access historical logs of transgressions.

The "burn book" could also be used for member-level infractions as well, local and remote, since suspending a single user (or a handful on a thousand plus member instance) might be an easier to justify decision than an entire instance.

## Transparency matters regardless of approach

{% figure "/assets/images/stickers/HowdySenil.png", "Senil pointing towards the viewier, winking. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

The thing that spurred the post that I'm even responding too is ultimately due to a massive lapse in transparency in an instance's actions. I will not comment on exactly why there was no communication when another instance was suspended - for very good reasons once that information came to light - but all I can say is that *something should have been said*. Given the severity of the now-suspended instance admin's behavior, it absolutely should have been suspended, even if it was just the admin.

However, there was no transparency in the matter. It took people questioning why links to the other instance disappeared for suspicion to be raised, up until the admin of the now-suspended instance made a long post talking about what happened, then explaining why the now-suspended instance was, well, getting suspended by others. I want to stress, **it is a very good thing this instance was suspended.** The admin admitted to being a pedophile, to keep things concise, though it isn't quite as straightforward as just that (mental health stuff played a role too, but we're getting into weeds that distract from my point).

The problem is that *nobody knew what the hell was going on.*

{% figure "/assets/images/stickers/SadSenil.png", "Senil curled into a ball, crying. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

This led to some uproar over the actions of the instance that didn't reveal anything at all when they acted, frustration over further decisions from that instance's admin team (which were 100% breaches of trust, but again distracting from the point), as well as a lot of calls to mass-suspend that instance over a lack of transparency. There were other matters brought up as well, however I personally saw zero direct evidence providing a basis for historical actions, with the only immediate one being "hey, you really broke trust here and that is Not Okay for an admin to do."

That isn't to say that it doesn't exist, but it's hard for me - a user who *might* become an instance admin himself - to trust that this is coming from a well-intentioned place instead of just lashing out. I did end up unfollowing and muting some who were causing this, largely because I just had no reason to believe their claims.

(The one that spurred that unfollow spree was someone who subscribed to the "local community first" approach, so that likely played a role in the actions, but that's me trying to prescribe meaning onto someone else's actions which is meaningless)

## What now?

{% figure "/assets/images/stickers/SleepySenil.png", "Senil sprawled on his back, sleeping. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

Well, I don't really have anything regarding "a way forward." The only thing I have to say is that the "local community first" approach doesn't *feel* like a true social media to most folks. Social media, is, well, social. It's a way to see what folks all over are doing, in addition to your good friends. There are existing places folks can exist in localized communities - however much I hate to say Discord and Telegram are big places for that, those are big places for that. Those spaces can't act as a gateway to other places, but they *are* still local communities

Trying to turn a federated instance into that - while still claiming to be part of the whole network - betrays the point of federating and encouraging folks to follow people on other instances.

It's difficult to follow hashtags and find folks from your circles if the people you follow can't really share much from outside *their* sphere, either. There are some folks on the fediverse that I found by happenstance, but that's because I'm on an instance that seems to take the "gateway first" approach that I personally appreciate. Even if it means it's more involved moderation-wise when it comes to decision making, it makes my time on the fediverse feel much more open.

I suppose this is also why I've kind of fallen out with tumblr. I really don't see many folks from outside my immediate circle and the folks in their circles. I have to actively hunt new folks down there, and I just don't have to do that as much on other sites. I've found artists who I never would have found otherwise. I've found folks who I'd at least consider loose friends right now. I've found others who I'd DEFINITELY consider very good friends.

I just... don't think I could ever get that from a *supposed social network* that fixates on local community first and foremost. But that's also just me. I'm not you, my preferences aren't yours. Maybe you love that approach. If you do, I'm somewhat surprised you've read this far. Have a hug, if you want.

## Last-minute addendum: Fedi v. Bluesky - FIGHT!

{% figure "/assets/images/stickers/AngrySenil.png", "Senil cracking his knuckles with flames behind him. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

I've seen talk as of late where folks lament over people going to Bluesky instead of the Fediverse at large, and I see *way* too many folks gripe over the fact that Bluesky is venture capital funded, or that it's controlled by one big company, or that it's protocol is built in a way where it's basically impossible for individual collectives to run, but a lot of y'all forget a crucial thing.

People don't care about those things - they want something that works *for them*. And while the Fediverse works for many - I mean, I'm here - it just doesn't work for many, MANY others. Either culturally (y'all need to get rid of the "I won't boost without alt text" attitude and ADD ALT TEXT TO REPLIES, same with wanting eye contact and food always CW'd), logistically (finding The Right Instance can be a pain, and also fuck you if you need a long-term presence on the network since you can't truly pick up shop and move between instances), and technically (federation is great but there are so many quirks to it that are a hurdle to many. See: how often you have to open a post on the original instance to get the full context of a reply chain).

*I* am one of the people who really doesn't care about the underlying protocol, the technical aspects (too much), or anything else that "makes federation better." I want something that feels right, that lets me hang out online, and just have a good time. I will still be here on the Fediverse - I still think the project has merit. But the culture here *has* to change for people to want to both come here *and* choose to stay here long-term, and make this corner of the net their primary space to be.

Otherwise, the Fediverse will forever be niche, closed off, and everyone here will continue to lament that nobody comes here and keeps going for The Big Network™, despite the eventual enshittification that *may or may not* happen to The Big Network™.