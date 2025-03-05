---
title: Negative energy prices don't mean what you might think.
date: 2024-11-24
last-modified-at: 2024-11-24
tags:
  - energy
  - capitalism
  - ramblings
---

I am begging people to understand this, because this is very important and yet I feel like few people actually understand the actual truth behind "negative energy prices". Contrary to what I see some folks (typically leftists and liberals) think, it has very little to do with capitalists being annoyed that they can't make money. It has everything to do with how power is generated, supplied, stored, and consumed.

Okay, maybe still a little bit of capitalists being angry they can't make money, but it's still not for the reasons you might expect.

The TL;DR is that "negative energy prices" mean that supply far outstrips demand, there is no way to store the excess power, and utilities have to **pay** clients - typically industrial - to spin everything they have up to full power to intentionally waste the excess energy so the demand meets the supply. Yes, waste excess energy, I am not joking.

If you want, [you can jump to where I talk about storing energy, the ways we can do it, and the future I hope unfolds.](#storing-energy-for-later). Otherwise, keep reading to learn what "negative energy prices" actually mean.

**Addition**: [I've also added some extra thoughts on energy](https://blog.senil.me/some-more-energy-thoughs/) that would've made this post even longer, and they're only tangentionally related at best anyways. They don't change anything here, it's just bonus content.

{% figure "/assets/images/stickers/HowdySenil.png", "Senil pointing towards the viewier, winking. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

## Power generation, consumption, and grid frequency

Both power supply and power demand tie into the fundamental required constant of the power grid - the frequency it operates at. In North America we use a 60Hz frequency, while Europe uses 50Hz. Various other regions use one frequency or the other, but the important thing is that frequency has to remain as constant as possible. Grid frequency gets measured to the thousandth of a Hertz in order to closely monitor grid behavior, and the power supply vs. power demand ratio determines how the frequency fluctuates.

An excess of power supply starts to bump up the frequency, while an excess of power demand decreases it. There *are* additional considerations such as the power factor - which is more or less a measure of how "efficient" your power transmission, distribution, and consumption is, but that's getting into detail that isn't relevant to "negative energy prices". The grid is surprisingly stable, but letting the frequency drift too far away from the nominal frequency of the grid can and will cause problems. Under-frequency (demand outstripping supply) can cause a wide-scale blackout if generators cannot keep up with the load in time, while over-frequency (supply outstripping demand) forces generation to shut off ASAP, something that's difficult for certain types of plants.

Solar facilities and wind farms can adjust their output relatively quickly, *however* it still has to be carefully timed to prevent an over-adjustment that'll cause a serious under-frequency event, which risks that wide-scale blackout problem. And in the event that a utility (or transmission company) *can't* shut power off fast enough, they're going to need to call up every resource they have to purposely waste power.

*Wasting* power is where the problem lies. There is no way around it, in a situation severe enough to cause "negative energy prices", load-shedding has to happen as soon as possible to prevent problems while generation properly adjusts.

There's just one problem, though. Solar facilities are very sporadic in their output power.

{% figure "/assets/images/stickers/ScaredSenil.png", "Senil with his hands on his head, mouth wide open in fear. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

## The unfortunate problem of solar

Solar power is *great*, especially as we get more efficient panels that can handle extreme heat better. But you have to pair solar power with some form of energy storage to help offset that sporadic generation - otherwise you run into a situation that California has dealt with, where they encouraged so many people to install rooftop solar (since rooftop solar alone is much cheaper than fossil fuels) **but** they neglected to set up the proper energy storage capacity to handle the fluctuations in power output. Solar facilities paired with quality battery storage - long-life batteries with high capacity promises even after a decade or two - are actually *more* expensive compared to a fossil fuel plant.

(aside: that doesn't mean we shouldn't install them, but it's a factor to keep in mind)

And, well, because they had no way to store all of that excess energy, utilities had to beg their industrial clients to spin up all of the motors, ovens, etc. that they could in order to waste that extra power. Power that they would normally be charged for, but because the utility is desperate to load shed beyond their normal capacity (utilities have some load shedding systems of their own), they generally have no choice but to *at minimum* pay for the cost of energy delivered to the clients they beg to waste power.

***That*** is what a "negative energy price" means. It means being forced to waste power because, for some reason or other, you're generating way too much power and can't get rid of it fast enough. On a per kilowatt basis, power is being generated way faster than you can get rid of it. The power grid *cannot* store power, power has to go somewhere. Trying to shove too much power onto the grid will result in that power finding its way back to where it was generated, since power has to make a complete loop somehow.

Power doing that in an uncontrolled manner means faults happening on transmission or distribution lines, transformers blowing up because they're being pushed well outside of their rated boundaries, substations going down, or generators potentially breaking because they're getting pushed too hard - *everything* runs at the grid's frequency whether you like it or not, and not everything is going to be built to handle an excessive over-frequency event. Stuff can - and probably will - break.

It's very expensive to fix these things. It takes time. It means large-scale blackouts if we can't fix it.

{% figure "/assets/images/stickers/AngrySenil.png", "Senil cracking his knuckles with flames behind him. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

## How to regulate generation

Not all forms of power generation can be quickly regulated and changed to new outputs. Nuclear is by far the easiest example of this - it's a great source of base-load power, but it's a pain in the ass to get it to some new power level. It takes a long time to increase or decrease a nuclear plant's output because, well, you're increasing or decreasing the heat generated by the radioactive material, and you *do not* want to even think of causing a meltdown by acting too fast.

Natural gas plants are able to change very, very quickly - just cut off the gas supply to certain turbine setups, or decrease the amount flowing in to cut back on the heat generated, slowing the boiling of water and thus the speed the turbines can move at. Wind and solar can also change very quickly, but by nature their output is less predictable. Sometimes you can have a good idea as to how much power they'll make, othertimes you just have to hope you're right and can spin things up or down fast enough to compensate.

For hopefully obvious reasons, the quickest way to guarantee power gets changed quickly is via natural gas facilities. But we *need* to phase them out as fast as possible across the world in order to cut down on greenhouse gas emissions - plus, y'know, we don't have infinite natural gas. So solar and wind renewables end up taking their place. But that means needing to install some sort of energy storage, either on-site or at dedicated facilities, in order to regulate their power output to better match the demand needed of them.

So... how can we do that?

## Storing energy for later

{% figure "/assets/images/stickers/DrainedSenil.png", "Senil lying face-down on the ground, with a low battery symbol above him. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

### Batteries

There's the immediately obvious solution to storing energy - just install batteries, silly! And you're right, standard batteries are a *great* way to store energy. However, pretty much everything on the power grid is expected to last decades, so whatever battery system you use needs to be able to retain the vast majority of its capacity after at least a decade, preferably even longer. Fortunately, there are new battery chemistries that are available today, or will be available soon, that are substantially more stable and handle charge/discharge cycles better than older chemistries.

The current hotness when it comes to stable batteries with long shelf lives are lithium-iron phosphate, usually just referred to as LiFePo. They currently have a worse energy density compared to traditional lithium-ion polymer (usually referred to as LiPo), however they trade that raw energy density for a much better "shelf life" in a way, with 80% capacities quoted after ten years. It's still a new chemistry, so we'll have to wait and see if that claim holds true in the real world. Oh, and LiFePo batteries generally don't need materials such as cobalt, which is difficult to source anywhere outside of the Congo, and cobalt is... not a conflict-free material, with mining of it being extremely manual labor intensive on the locals. Expect LiFePo to show up more in large packs, such as EV's, too.

There also exist a variety of *sodium-ion* batteries, too, that are gaining interest. To my knowledge they aren't remotely as common as lithium-based batteries, but their properties are similar enough to lithium-based chemistries. The use of rechargeable sodium-based chemistries is extremely recent, however we'll likely see it proliferate over time, too.

### Pumped Hydro

But batteries aren't the only way to store energy. We can store energy in the form of gravitational potential by holding some material of some kind higher than some other location. Well, that's energy we could store by pushing something higher up, and get back by letting it fall down and spin a turbine in some form. The way we currently know how to do - and have done for well over a century know - is pumped hydro.

The idea is relatively straightforward, though difficult to implement. Find two conveniently placed lakes, and set up a hydro facility at the lower one, running the usual tubes and piping from top to bottom. This way, you can generate power by "pulling" water from the higher lake, using its potential energy to convert into electrical energy from its kinetic energy going past the hydro turbines. A pumped hydro facility will *usually* do this during the day, selling power when it's needed more. And then, when power demand is lower, a pumped hydro facility will then buy power back in order to shove water from the lower lake back up to the higher lake for future use the next day.

This system is remarkably simple and effective - it's more or less a glorified hydro plant, just with the need to set up a way to push the water back up the hill. While I have no experience with a pumped hydro plant, one way you *might* be able to accomplish the "pump water back up the hill" would be to use the very same generators used when the water flows downhill, which is possible because of one neat trick. Generators and motors are the exact same thing, just wired the other way around.

{% figure "/assets/images/stickers/ConfusedSenil.png", "Senil dazed and drooling, with a loading icon above him. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

If you could change the wiring on the fly (letting the generator safely stop before doing becoming a motor, and vice versa), you could theoretically use that generator to push water back up to the higher lake. The generator-slash-motor would need to be powerful enough to accomplish such a feat, so it's probably more realistic to just have a separate pump system. It'd cost more, but it also means you don't need to spend more on a generator that'll be strong enough when used as a motor, let alone install it in the right place.

Pumped hydro does have a fundamental flaw, though, and one you might have figured out by now. You need convienient locations to install such a system. Two lakes that are large enough, with enough of a height difference to give a substantial amount of potential energy, and close enough to minimize material costs. Sure, you *could* terraform to create artifical lakes to do this, but that's pretty damn expensive just to use pumped hydro instead of batteries.

### That weird crane thing

There's been an idea for years now that works effectively the same as pumped hydro - lift some stuff up high enough to store substantial potential energy when power is cheap, and carefully lower them down to spin a generator when power is needed. These designs typically work by lifting and stacking concrete blocks, but there's some flaws with this system in my eyes.

First of which being that you lose out on potential energy if you can't stack enough blocks safely. You only get the maximum potential energy when you can stack multiple blocks at the highest defined limit, while pumped hydro gives roughly the same potential energy throughout. There's also of course the risk of breaking the concrete blocks, either from the crane being too rough with them, a storm potentially knocking the higher-up ones down, or the blocks just wearing down with time.

As far as I'm aware, this idea hasn't actually been installed in the field, only tested by various researchers and companies to determine viability. With battery banks becoming cheaper over time, I personally don't see this weird crane idea coming to fruition and being installed grid-scale just to avoid batteries. To me, it feels far too risky and with not enough reward compared to any pumped hydro facility, let alone a dedicated battery facility.

{% figure "/assets/images/stickers/SadSenil.png", "Senil curled into a ball, crying. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

## Where does this leave us?

Ultimately, the inabilty to store enough energy causes problems with the grid. We cannot just install renewables without considering this factor, unless we collectively accept that wasting potentially tons of excess energy is worth the effort to install a ton of solar without any way to store power (even on-site). This inability is part of why I dislike rooftop solar if it's not paired with an on-site battery system, because unless the solar panels are prevented from feeding power to the grid, utilities have this extra generation that they might not know what to do with.

One individual home isn't going to make much of a difference, but thousands of homes with a couple kilowatts of solar panels starts to become a problem.

I want us to learn from the past and prepare for the future. Electrification is only going to continue, and we should prioritize minimizing our need for electricity in the first place too. Installing heat pumps to move more energy than it takes to run them. Building out quality electric-powered public transit in urban areas that cuts down on the need for EV's in urban areas in the first place.

And I want folks to read past the god-damn headlines, read the articles and studies, and not make wild conclusions without knowing what the hell they're talking about. Hell, most of this is me shooting from the hip too, I don't expect you to believe me or trust my input. I just hope some folks take something away from this long as hell post.