---
title: Rest in peace, Cohost
date: 2024-10-25
last-modified-at: 2024-10-25
tags:
  - social media
  - cohost
  - ramblings
---

Cohost is shutting down the end of the year. While I’m kinda sad because it was a good experiment to see if non-federated social media could be viable that doesn’t rely on selling data or anything, I think Anti-Software Software Club just made too many assumptions that didn’t or couldn’t pan out. Including just… not understanding what they wanted in the end.

This post was originally a three-part tumblr post, so it's very long. Part "one" was what I think went wrong, part "two" is why I think a federated model "works" a bit better than centralized (though it's flawed, too), and there's a "TL;DR" part that [I'll just link to here if you want to skip the many, many paragraphs below.](#the-tl-dr-of-my-thoughts-re-cohost-shutting-down)

## What I think they assumed

Number 1 mostly being them being “blindsided” by Stripe clarifying their policy that, in the end, means ASSC couldn’t use them as a way for users to tip each other or the Artists Alley section and such. That policy existed for years, well before Cohost ever existed. For context, ASSC originally wanted to build a Patreon competitor, not a social media site. They would have failed so hard if they stuck to a Patreon competitor on this alone.

And in my opinion, number 2 is their pay. They were paying themselves very well-off all things considered, and everyone was paid the exact same amount (~94k last I heard). That's… a lot of money going towards pay that could’ve gone to hosting costs. They’re a startup. You pay yourselves what you can. I appreciate that they paid themselves well, but again. Startup. You pay what you can, and they were nowhere close to breaking even at any point.

I think their financial model didn’t do themselves any favors - they started out with “we got a lot of loan money to do this and now we have to make it profitable” which, yeah, sometimes that’s what it takes. But that’s venture capitalism. Especially since Cohost’s source code WAS the collateral! They acted as a leftist group trying to market themselves as a non-profit/not-for-profit (they’re a LLC, they’re legally not forced to do either), paying themselves well more than they realistically, and hoped they could get enough people to subscribe monthly to break even.

**That… doesn’t work.**
{% figure "/assets/images/stickers/DrainedSenil.png", "Senil lying flat on his stomach. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

Not to say this would’ve fixed things, but I think them registering as an LLC didn’t help. That prevented them from bringing on anything resembling a volunteer, and since their whole thing was “everyone gets paid the same” it meant they had to operate with very few people. If I recall correctly, they had one moderator. Maybe two. Maybe. Two developers, an artist, and a moderator. Four people. MAYBE five, I forget the exact number.

## Hypothetical territory ahead

Being a non-profit comes with its own set of problems, but if they could become and maintain a 501©3 non-profit, they could pay themselves what they could and have people willing to help volunteer moderate. They could never get code contributors, though, since their source code was their collateral it by nature had to be closed off. Also, donations (recurring or one-off) are tax-deductible for US-members, so while it’s not a HUGE benefit it offers at least that small bonus.

I’m glad that they tried, and got as far as they did (even if it meant loan after loan to not die instantly). It showed that it could be possible - that there’s hope in this idea. It’s just a question of HOW to make it a sustainable reality. I don’t think there’s a clear answer there, though. Like my non-profit idea hinges heavily on maintaining 501©3 status (or similar) and being able to bring on volunteers as-needed. Using a public spec for the back-end (like ActivityPub or ATProto) so the focus can be on implementing it (even if federation is never a thing) instead of doing it raw - which avoids the back-end development time but then means having to work with an existing spec that may or may not change substantially over time.
{% figure "/assets/images/stickers/SadSenil.png", "Senil curled into a fetal position, sobbing. Art by [Dragonjourney](httpss://x.com/Dragonjourney)" %}

I don't know. I have no idea what would make a medium-form social media such as Cohost viable. Maybe it’s the same idea but with lower pay so it’s easier to bring new people on as-needed, with the expectation that this is a passion project ‘til it gets off the ground. Maybe it takes the “use a public spec for back-end” approach and focuses on the implementation of it with their own additions and flair. ActivityPub is one spec, but you have Mastodon, Pixelfed, Misskey, Wafrn, etc. that all go in different directions. ATProto will likely be the same one day - Bluesky being the obvious “reference” implementation right now, and then various other flavors that go their own direction with ATProto down the line.

Maybe it’s something else entirely that I could never ever think of. All I do know is that I’m glad they tried. Unfortunately, the writing has been on the wall for months now and honestly? If you didn’t expect that, that’s on you. People have been saying that Cohost wasn’t sustainable for months.

## Why I think the federated model "works" (kind of)

So part of what makes the fediverse (Mastodon, Pixelfed, Misskey & co., Wafrn, etc. for your Twitter/Instagram/Tumblr vibes) work from a financial view is that costs are spread out across tons of instances, and there are tons of ways to host this stuff. Either from a dirt cheap VPS from Hetzner that hosts a dozen people, to a hundred-ish instance that runs locally with solid redundancy, to a thousand-ish instance that ALSO runs locally (but is suffering growing pains from VPS to local transition IIRC), to a multi-thousand user instance that runs on… something? I don’t know what meow.social uses.

But those costs are on a per-instance basis, and there are tons of ways to shift that cost perspective around to make things cheaper, or accidentally make things more expensive. Using a more costly VPS service, expensive S3 storage, expensive CDNs to make stuff available more better (extra useful for those huge instances that cross the thousand-member mark), etc. There are various ways to make it expensive.

{% figure "/assets/images/stickers/ScaredSenil.png", "Senil screaming in fear, hands on his head. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

But there are ALSO various ways to make the hosting cost go down. Running local boxes means the only hosting cost (outside of external S3 buckets, CDNs, etc.) is the up-front purchase cost of hardware, upgrades over time, and your time-cost of keeping them running (though you might be able to make it set-and-forget enough to where a VPS might be set-and-forget). Forgoing S3 buckets and a CDN mean everything goes through your local boxes, which’ll up local storage needs but again, those are up-front purchases (though you might need to upgrade to small business internet to keep your ISP happy, which I guess counts towards hosting costs but you also live there so…)

This is, of course, only considering hosting stuff. Pretty much all fediverse instances, as far as I’m aware, run on totally volunteer labor. These instances are passion projects of the admins and mods, run for the sake of running it and to provide community to folks online. If you were to start paying for their time administrating and moderating, then you start to see instance costs go higher and higher (varies on what instances pay folks, how they handle time spent, etc.). That IS a part of the equation that the fediverse does not explicitly handle.

The same “passion project” logic is a large part of fediverse softward development outside of the big projects like base Mastodon and *maybe* Pixelfed - those are developed in large part by actual organizations who pay people to do the bulk of the work. But here’s the kicker - other people can also help out. Submitting feature requests, bug fixes, issues, etc. to the teams directly means there’s a chance of problems getting fixed or features added that other developers have the passion to show how to implement it, or discuss how to handle it with the folks who run the project.

That’s of course something Cohost could never benefit from, because the source code itself was used as collateral for their initial loans. They could never open source it under any terms without the express permission of the loaner, who would likely veto the idea anyways, because there goes the motive to keep it as collateral. They can’t have other people contribute bug fixes or program new features to help them out.

## Paying people to run a service is important

{% figure "/assets/images/stickers/HowdySenil.png", "Senil pointing towards the viewer, winking. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

Cohost does have the benefit of, y'know, paying everyone for their time and energy… but that costs money that I don’t think they considered how to structure. They only ever had one, maybe two moderators for THOUSANDS of users. Yeah, they’re paid, but they literally only have so much time in a day to moderate things - and they can’t be awake 24/7 to watch over things, while volunteer mods might be in various time zones or have different work schedules so there might always be a person or two to monitor stuff.

I know there’s nothing that can really bridge that monetary gap - paying people and everything around that costs a lot of money, which can scale way faster than hosting costs. The instance I’m on (which shares staff and such with another instance and a Lemmy one so it’s not super fair) has seven people listed as staff. I don’t know how much work they actually put in (or need to put in) to moderating and administrating everything a week, let’s just go with 20 hours a week per person, or 140 hours total per week.

At my state’s minimum wage (bout $16 an hour right now) that’s around 116.5k annually, or 9710 a month, give or take. I don’t know the exact hosting costs since IIRC stuff is now hosted locally, and I don’t know what additional regular “costs” exist beyond whoever’s basement this is all at, but whatever it was it now requires an extra 9710 a month to break even.

We have a listed “active user count” of 844 between furry.engineer and pawb.fun - I’m not counting the Lemmy instance because that’s a much harder figure to find. I’m also assuming there are zero duplicate accounts between the instances, and everyone is totally unique. In order to raise enough money just to pay every my state’s minimum wage at 20 hours a week (treating this as a part time job, basically), each member would need to contribute about 11.5 bucks a month to just pay the staff team for their admin and mod work. Probably add in a couple more bucks to help cover any added costs like better internet, increased power bills, etc. and suddenly you might be looking at 15 bucks a month to pay everyone a minimum wage part-time job’s worth of labor and help cover self-hosting fees.

That’s not a lot of money all things considered - since this is a passion project of sorts I don’t expect this to be a full-time job, especially since nobody is really doing active development work like the Cohost team was doing. But that’s still money to keep it up and running. BUT! There’s a small beauty in all of this.

### Larger instances don’t necessarily need a ton more mods or people behind it.

Take meow.social - a furry instance with about 2.3k active users. I don’t know how exactly they host things, but they have a transparency report that goes over what they raise via Patreon monthly as well as their expenses, and it seems like it trends to around 300 bucks a month for hosting and such. They have two admins and four moderators - taking my same “part time job, my state’s minimum wage” estimate, we’re looking at an additional $8320 a month to pay everyone. Let’s round up that plus the rough hosting cost of 300 to a straightforward $8700 a month. Recall that they have 2300 active users. If every active user donated to meow.social to pay their staff and keep it running, **they’d only need to donate $4 a month on average to keep it going.** Toss in some extra to help build up a small savings for future upgrades and badabing badaboom, you have a functional instance running at not that much all things considered.

Meow.social is based in France though, so the reality is these numbers are probably low but the point remains that staff plus user count doesn’t have to scale that much, but you should still have plenty of mods to be effective.

However, meow.social is still a passion project - everyone part of running it has real jobs outside of it, the paying part is just a “thank you” of sorts to help cover their time and reward their efforts. And that’s kinda the bridge between fediverse projects, which are generally run as a passion project and any donations/payments are a “thanks for keeping this going” deal. While a brand-new social media, which has the development costs of building the damn thing on top of hosting and paying people, is GOING to cost more money because you have to pay for the development work too, which is definitely a full-time job that’ll have to pay decent enough to entice people to work there and stick around.

It’s why I mildly get the Cohost team paying themselves well - it’s not exactly easy work doing all of this. And it’s not like I know their exact numbers on hosting costs, development time, legal fees, etc. that factor into everything. But I still think that maybe there was something that they could’ve done differently to stay on top of things better, and maybe. Just maybe. Pull off the ultimate mission of “making centralized social media that doesn’t suck for users.” That’s why I applaud the Cohost team for trying, and succeeding (ish) for so long.

**They suggested that this might actually be possible, if things worked a little differently.**

{% figure "/assets/images/stickers/ConfettiSenil.png", "Senil happily tossing confetti in the air. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

## The potential of Cohost

Put more effort into the core product and fixate on one idea instead of trying to come up with a different one, leaving the core product untouched for months. Maybe use existing back-ends to kick-start development, so that you aren’t building entirely from the ground up and have reference implementations of various things to help get the project going (aka my idea of using ActivityPub or ATProto as the back-end, with the intent of never allowing federation). Paying yourselves a bit less to compensate for “this is a start-up effort” and prioritize having more of the support crew as-needed.

I know that there’s potential here. I don’t know how to go about it, or if it’s even worth the initial investment to try, but I at least think that it might maybe be viable. It’ll take some clever thinking, but ultimately Cohost was a starting point in the effort to return to a less-scummy web. They started the path to proving it’s possible, even if in the end they failed. Hopefully some other crew picks up the torch and goes farther, having learned from what likely did Cohost in and doing better.

Ultimately, there’s just no way to possibly know. All I want is for folks to have more spaces online that aren’t data-selling hellholes like Facebook/Instagram/Threads, Twitter, Tumblr, probably Bluesky eventually (if not already), Reddit, TikTok, etc. There aren’t many well-known medium to large online spaces that are run by the people, for the people anymore. It’s all about “line go up” forever to please shareholders and venture capitalists, not breaking even while running a satisfying service.

While I think the fediverse proves a different direction that social media could take, being a source of passion projects and the occasional corporate group paying folks to develop key pieces that help everyone else, there is still a place for more centralized social media. The fediverse has its own problems too, both structurally and socially.

{% figure "/assets/images/stickers/ScaredSenil.png", "Senil screaming in fear, hands on his head. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

# The TL;DR of my thoughts re: Cohost shutting down.

OK this is still a long TL;DR but I tried OK?

- Cohost is shutting down end of the year, going read-only October 1st and getting data backups out the door ASAP. In my opinion, this was going to happen eventually given their funding model - so it was a question of "when", not "if" it happens.
- Despite the flaws I saw in how Anti-Software Software Club marketed themselves as a company (being leftist co-op not-for-profit despite being an LLC with no obligation to do that), there was still value in what Cohost was trying to do.
- Them incorporating as an LLC, to myself, might have been a mistake since it legally prevented them from bringing on anything resembling volunteer moderators. While being a 501(c)3 or similar non-profit is difficult, they could still pay the core team and have volunteer mods if needed.
- Their initial round of funding used the Cohost source code as collateral, preventing them from making it open-source to help gather community contributions to bug fixing, feature requests, etc. on the back-end directly.
- They wildly misunderstood Stripe's terms of service when it comes to payments, forcing them to gut months of work into "eggbux" which is basically what tumblr tipping is, and was part of their effort to become a Patreon alternative (their original goal). They claim this was a sudden change, despite it just being a language clarification for a policy Stripe has had for years now.
- Per the leftist co-op branding, they all agreed to pay themselves equally (for the most part, stuff has changed now and then) and increase their pay to align with cost-of-living adjustments. This, to me, is a noble goal, but contributed to the vast majority of their expenses and made it even harder for their user base to subscribe and help cover operating costs.

### Despite all of these negatives, they still managed to...

- Prove that this is a viable concept - Cohost has INCREDIBLE subscriber rates for people who are willing to pay for the service to keep it alive. This, to me, heavily suggests that people want not-scummy social media that doesn't sell user data or push shitty ads.
- Prove that users like this kind of service. As far as I'm aware, there was no advertising for Cohost outside of word-of-mouth. Everyone who signed up likely heard of it from someone else. This of course weakened new user rates, but it also meant every active user there heard of it from someone and liked it enough to stay.
- Prove that it might just be possible to do all of this work and pay their core team. That idea alone likely led to more monthly subscribers willing to help keep it afloat, because they knew their money was also helping keep them paid too. I still disagree with their payment model and motives, but hey. They still did it.

{% figure "/assets/images/stickers/FlexingSenil.png", "Senil flexing his biceps, smirking. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

**Cohost, despite its flaws, was a fantastic experiment.**

I'm sad that it's gone, but happy for what it was able to achieve and suggest is possible for future projects. I don't want people to be disheartened by Cohost's attempt - I want people to see what they did, try to understand the core pain-points, and try to get farther than ASSC did with Cohost. Maybe we'll have a true, not-scummy centralized social media competitor someday, because people dare to keep trying to make the dream real.

Will that ever happen? Time will tell. But I don't want folks to ever give up. The web can still be ours, one made for the people, by the people, instead of for venture capitalists who want more money forever and ever.