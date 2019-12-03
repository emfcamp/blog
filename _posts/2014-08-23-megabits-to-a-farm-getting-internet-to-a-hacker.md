---
layout: post
title: 'Megabits to a farm: Getting Internet to a hacker camp'
date: '2014-08-23T14:37:00+01:00'
tags:
- emfcamp
- noc internet network
tumblr_url: http://blog.emfcamp.org/post/95545988673/megabits-to-a-farm-getting-internet-to-a-hacker
---
In [our last post](https://blog.emfcamp.org/2014/08/18/how-to-network-a-field-internet-to-the-tent-at/), we discussed how the network is distributed both wirelessly and wired around the site. Here we’ll look at the other side of the equation: how the network is brought to the field in the first place.

## It’s a tall order
In an ideal world, these events would take place in fields next to large data centres. But as parking lots aren’t usually great for camping, there’s always the challenge of getting Internet access to the site in the first place.

Last year our peak usage was about 140Mbps 5-minute average, and roughly symmetric usage. This time we’re expecting three times as many attendees, so at least 420Mbps. Actually, now that the word is out about EMF, we are expecting a higher proportion of campers who are used to the European hackercamps where bandwidth is plentiful, so the bandwidth required is likely to be even greater.

Of all the available access technologies, we could immediately discard most due to being unable to provide enough throughput (ADSL, FTTC, EFM, and so forth), which left us with just two: radio and fibre.

![Fibre cables being spliced](/images/tumblr_inline_p8ne7k7nKM1rpuop0_500.jpg)

Fibre circuits have a minimum term of at least 12 months, and high excess construction charges if fibre doesn’t already exist (such as at a remote farm). And, unless the site is on-net with a carrier’s existing network, it’s always going to rely on Openreach products for the last mile.

EMF is in an awkward position where it has enough attendees that it has high bandwidth requirements, but not enough that the budget can stretch to a 12 month fibre contract without major sponsorship, which wasn’t forthcoming this time around (if any carriers who read this would like to help out in 2016, do get in touch!).

This left us with radio.

Telehandler Operator Will Hargrave was quoted after EMF 2012 as saying “I’m never doing microwave again”. But as this was the only remaining option, and he had plenty of hair left to pull out, we had to try.

## Big masts
![A radio mast being erected](/images/tumblr_inline_p8ne7kLUOQ1rpuop0_500.jpg)

We’re putting a 30m mast up a hill on the site and cabling this back to the on-site NOC data centre, housed in a 20ft refrigerated container. However, this year we’re the opposite side of Milton Keynes from before, so we needed a new location to run the radio link to.

[Colocker](https://www.colocker.com) is a new data centre in Milton Keynes that provides lockers for colocating servers. They’re letting us put the other mast up in their parking lot and are generously providing a pseudowire back to Docklands.

So from the NOC-DC, we run fibre up the hill to a mast, radio over to Colocker, copper into their data centre, and then a 1Gbps pseudowire down to Telehouse.

## Big radios

![Radios being attached to a mast](/images/tumblr_inline_p8ne7ku1JU1rpuop0_500.jpg)

We’ll be using DragonWave radios again in Ofcom-licensed frequencies. Initial results from the survey last week indicate that we should be able to get around 436Mbps from each radio each direction to/from site, however there are line-of-sight issues that we hope to solve with a taller mast.

[Bitlair](https://bitlair.nl) are also bringing a pair of Ubiquiti AirFiber units running at 24GHz that we’ll have available as a secondary/backup link.

## Transit
As is now common with these events, we are running a multi-homed default-free BGP network under our [shiny new AS60079](https://stat.ripe.net/AS60079). We’ll be taking transit from [AS42579](http://www.sargasso.co.uk) Sargasso Networks as well as peering with other ISPs at [LONAP](https://www.lonap.net/).

It’s also traditional to run a publically-addressed network with no NAT and no network-level interference in the end-to-end data path. This means that each and every device for each and every attendee gets a public IP address. It also means we don’t run any kind of firewall or interfere with or inspect your packets in any way - those of you used to having a NAT “firewall” protect you from attack had better [be prepared](https://wiki.emfcamp.org/wiki/Network#Security).

Naturally, IPv6 is enabled throughout the network and should “just work” for everyone. If you encounter any problems, we do recommend that you don’t disable IPv6, but instead try to understand what has gone wrong and fix it - the InfoDesk can help here. The 21st century is when everything changes, and you’ve gotta be ready.

## More information
There’s more information on how to use the network, including a few “do”s and “don’t”s, on [our wiki page](https://wiki.emfcamp.org/wiki/Network).

Have a question? Drop us a line at noc@emfcamp.org or [follow us on Twitter](https://twitter.com/emfnoc).

## Sponsors

![Image of Colocker](/images/tumblr_inline_p8ne7llpf81rpuop0_500.jpg)

We’re especially grateful to Colocker for arranging the transport down to London. If you’re looking to host servers on the Internet, [check out their new concept in colocation](http://www.colocker.com/).
