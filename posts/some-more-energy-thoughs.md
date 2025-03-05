---
title: Just some more energy thoughts.
date: 2024-12-04
last-modified-at: 2024-12-04
tags:
  - energy
  - ramblings
---

This is a *slight* continuation of my very long post on ["What negative energy prices really mean"](https://blog.senil.me/what-negative-energy-prices-really-mean). I want to talk more about my stance on rooftop solar (either residential or commercial), electrification as a whole, and such.

There was originally a whole bit about power factor and whatnot, since I did briefly mention it there, however I can't distill it into an easy to understand formate just yet, so it's being left off for later. Anyways, let's get on with it since this is already disjoint.

{% figure "/assets/images/stickers/HowdySenil.png", "Senil pointing towards the viewier, winking. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

## Solar and battery banks

It's totally possible to add battery banks to existing solar plants, there isn't a significant reason to not do so, and it's something we need to be doing as soon as possible to help make solar more controllable and thus viable. This is also why I think any form of rooftop solar needs to be accompanied by battery banks. Even if a utility pulls excess power from your battery bank (something that would be *really neat* to somehow implement, again with my idea of stuff having some percentage of excess "invisible" capacity that never matters to the end user), it's still a controllable amount of power that they can pull.

I personally plan on installing rooftop solar with battery banks someday, primarily to enable any self-hosted equipment to continue to operate in the event of a blackout (even if it's just to safely backup locally and shut down to help conserve overall power), but also to cut down on the costs of running powerful equipment if I ever need that kind of raw compute strength. [I've specced out a very powerful home NAS system](https://newegg.io/cad80e7) that is 100% excessive and I will almost certainly never build, and at that point it'd make more sense to build a full-on server rack with more modular components, but it'd be really fun anyways.

Having a battery bank on-site would also be helpful since it means I don't risk back-feeding power to the grid unless the utility wants me to. All rooftop solar systems, or even generators for any building, need a disconnect switch from the distrubition system to prevent backfeeding power to the grid. This is for safety reasons, to protect lineworkers while they make repairs. The last thing they need is to be working on live lines that they don't expect, which could cause serious harm to them or the equipment they work with.

{% figure "/assets/images/stickers/ScaredSenil.png", "Senil with his hands on his head, mouth wide open in fear. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

## Expanding electrification

As we shift away from natural gas and fossil fuels in general, the grid is going to need to keep up with the rapid pace of electrification. This does present some serious problems, since it takes more time to upgrade the grid, add generation facilities, improve transmission lines, substations, etc. than it takes for homes to become electric-only and ditch natural gas or propane. This is why I think we need to focus on cutting back on how much power is needed at all.

Well, how do we go about doing that?

### Insulation and heat pumps

The biggest problem, when it comes to buildings, is *insulation*. A poorly insulated building is going to let more heat in or out compared to a well insulated building, it's just a factor of the physics around heat transfer. Every problem when it comes to heating and cooling buildings of any size is made much easier when they're better insulated, and require less effort to heat and cool. Literally nothing else matters if buildings are poorly insulated, even if a home doesn't electrify their heating. A gas-fired central furnace will need to be sized larger and/or run for longer than a home that's much better insulated.

Outside of insulation, this is where heat pumps come in. Electric resistive heat is 100% efficient - every watt that goes in is a watt of heat shoved out in some way, shape, or form. Transmission, however, is *not* 100% efficient, let alone power generation itself. Heat pumps are miracles of refrigeration, and they aren't even new. Air conditions *are heat pumps*. Your fridge is a heat pump. We use heat pumps regularly, but we haven't started using them for, like, heating until very recently. They can move upwards of four times the energy it takes to run them, which can easily beat out electric resistive heating, and usually beats out natural gas heat. Plus, you know, they also cool your home in the hot spring and summer months.

And also the whole dehumidication thing, that's a nice bonus in some places.

{% figure "/assets/images/stickers/LaughingSenil.png", "Senil laughing on the floor. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

Heat pumps in general only out-perform a condensing gas-fired furnace (it just absorbs more energy from the created water vapor that's otherwise wasted) if their coefficient of performance - the measure of how much heat energy they transfer compared to the power they draw - exceeds something in the neighborhood of 2.4, or 240% of their input power. Otherwise, it loses out to natural gas due to transmission losses and such, especially compared to how efficient higher-end furnaces get.

On a wildly different note...

### EV's and public transit

A big problem I take with EV's as presented in the United States specifically is that they're being treated as the exact same as gas and diesel powered cars. The idea is that everyone just replaces their fossil fuel powered cars with an EV and we call it a day. This... is a big problem. When it comes to the local problems, it's adding a sudden burst of electric load to the grid that may or may not be able to handle it.

There also, of course, the problem of mining the materials in the first place. Mining is destructive, and we still only have so much raw material to build batteries - battery recycling helps, but if everyone is driving an EV with 60+ kilowatt-hour batteries, it's still a huge amount of raw material to mine in short order. Those batteries still need to be replaced over time, as well, and batteries make up the BULK cost of an EV, to where it almost makes more sense to *buy a new one* (even a gently used one) than to pay for a totally new battery. Especially in a day and age where EVs are improving at a breakneck pace.

{% figure "/assets/images/stickers/ConfusedSenil.png", "Senil dazed and drooling, with a loading icon above him. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}

Due to this rapid development of EV personal vehicles, I just can't really recommend them being *the* way of transit. Let alone the fact that all it does is trade one problem for another, while avoiding the problem of "one more lane" and constantly new road infrastructure that's needed to support more and more vehicles on the roads and highways. The solution to that is public transit, to nobody's surprise.

Even a battery-powered bus can transport way more people than the equivalent number of EV's, plus an aged battery could be straight-up used for general battery backup storage with some re-design efforts from the existing cells. Light rail, trolleys, and even commuter rail would massively benefit from being electrified. Any form of long-distance rail - medium or high-speed - needs to be electrified as well in some way, shape, or form. Most engines are diesel electric hybrids, which is a start, but full electrification of passenger trains would be *huge*, and be a massive improvement from everyone just owning EV's and having thousands and thousands of fast-charging stations dotting highways nationwide.

## Closing off

The moral of the story is... well, there isn't one. I don't really have a neat and tidy way to clean this up since it's a disjoint ramble about some stuff that should make electrification easier, as well as what I plan on personally doing should I have the money to both own a home, and make those kinds of upgrades. I just needed to get this off my chest and into one addendum piece so it's all in one place and I can hopefully just reference to this later down the line.

Thanks for reading this far, I guess.

{% figure "/assets/images/stickers/FlexingSenil.png", "Senil flexing his biceps, smirking. Art by [Dragonjourney](https://www.furaffinity.net/user/dragonjourney)" %}