---
layout: post
title: 'The Internet: EMF Delivers'
date: '2018-08-21T14:54:53+01:00'
tags: []
tumblr_url: http://blog.emfcamp.org/post/177236383588/the-internet-emf-delivers
---
At the first EMF in 2012, the quality and throughput of the internet connection (and wifi) was well-received and [apparently a pleasant surprise](https://twitter.com/Ash_Force/status/242067006537474048). Of course, having set a high bar, we’ve taken pride in improving the performance, whilst streamlining the process at each subsequent event. Each year we’ve [talked about the challenges we’ve faced doing this](https://github.com/emfcamp/emfnoc#presentations).

Unsurprisingly this has led to the Internet connection being a factor in choosing the event site: weighing up the viability of getting a suitably impressive connection two years in advance of the event, without knowing for sure what’s possible.

![A cherrypicker installing a wireless link at EMF 2014](/images/tumblr_inline_pdtb2l2opk1rpuop0_500.jpg)

We’ve never really wanted to do wireless point to point links, but this was usually driven by necessity. Data circuits of any significant bandwidth and distance have a minimum contract of 12 months from any provider in the UK, and this has never been something we felt we could justify putting in the budget, as our policy is to keep ticket prices as low as possible so that as many people as possible can attend (as a point of reference, the network was 4% of the total event budget in 2016).

In 2016 we finally achieved “plug and play” fibre by virtue of having the event right next door to a well-served business park.

![Presentation slide showing "Mission Accomplished"](/images/tumblr_inline_pdtb3fbkCe1rpuop0_500.png)

This year we have a lovely site but really not a useful location for the internet. Those of us who’ve visited the town have already experienced the almost complete lack of mobile coverage and shockingly poor DSL. The hilly surroundings of the site would make any wireless connection an exercise in frustration - even if there was somewhere useful to get to.

So planning for alternatives began a year ago, and this time we’ve had to do the previously unthinkable - pay for a circuit. Not a huge distance mind you, and not at retail prices, but as other options were delayed and ceased to be viable, this route became inevitable.

We’ve been amazingly lucky though to have Sky’s sponsorship and cooperation in making this happen. Our circuit runs to their nearby point of presence, and they’ve used their [Sky For Business Ethernet](https://ethernet.business.sky.com/) product at no charge to bring the connection back to our router in London’s Docklands, at the heart of the UK internet.

![Network diagram](/images/tumblr_inline_pdtbw1VlFI1rpuop0_500.png)

In London, our router is again being kindly hosted by [LONAP](https://www.lonap.net/), who are also interconnecting us through their IXP to our peers and transit providers.

## The circuit on site

Fibre circuits need to be delivered somewhere - the provider installs equipment at each end of the circuit to monitor and troubleshoot it, so it’s not as simple as them leaving a fibre coiled up somewhere for us to plug in. It needs to be in a clean, dry, powered, secure, permanent location.

Somewhere close to site, ideally on the correct side of the road; somewhere we can run power to, but not so far from the road that we end up paying large construction charges. Hence we were on site for a few weekends in January to [build and install a green street cabinet](https://twitter.com/emfnoc/status/959510197046784002) ready for the circuit to be delivered into it. This marks the first permanent EMF installation! During subsequent visits we’ve run power to it and trenched ducts out to the road for providers to hook up to. (Our thanks to [Envico Engineering](http://www.envicoengineering.com/) for selling us the cabinet at cost).

![Base of the network cabinet being installed](/images/tumblr_inline_pdtb4npqOR1rpuop0_500.jpg)

We anticipated some delay in providing the actual fibre, which is why we started this process early, but not quite as much as a delay as we ended up having. The circuit was finally completed at the end of July though, so no fingers pointed here.

We left a router installed in the cabinet too to allow us to test it - happily everything is working as expected and we’re getting a [full 1 Gbps back to London](https://twitter.com/emfnoc/status/1025396182816833537).

![Speed test showing 1Gbps](/images/tumblr_inline_pdtb4wDBcZ1rpuop0_500.png)

Having the circuit not only installed but tested a full month in advance of the event has provided some great peace of mind for [the NOC team](https://wiki.emfcamp.org/wiki/Team:NOC), and we can now go back to preparing other crazy plans, like running 1.2km of fibre underground up to the camp site!

We’ll be doing [a presentation as usual](https://www.emfcamp.org/line-up/2018/71-emf-2018-infrastructure-review) on the Sunday afternoon, with more details about the network, voice, power and video systems and how you used them. Here, we’ve only talked about the uplink, but our presentation will also include details about how the network is distributed around the site.

## Using the network
Once at EMF, you can connect to the **emfcamp** wireless network with username **emf** and password **emf**. If your device doesn’t support this, there are other options which are [all detailed on our wiki page](https://wiki.emfcamp.org/wiki/Network), though we don’t recommend them as they are less secure or have poorer performance.

Around the site, you’ll find a number of locked loos that we use as weatherproof network distribution points. We call these “Datenklos” or “DKs” for short. If you’re looking to connect with a wired Ethernet connection, just leave your cable outside and someone will plug it in for you. At the end, leave the whole cable coiled outside and it will be disconnected. (Not happening fast enough? Everyone at EMF is a volunteer; drop by the [Volunteer lounge](https://map.emfcamp.org/#19.18/52.0398503/-2.3768114) and volunteer your time!)

The same applies for UK 13A (BS1363) power cables, although we recommend you bring something with a blue 16A IEC60309 plug (a.k.a. Commando or CEEform) if possible, as you can plug these in yourself. Avoid any uncovered adapters that might get wet. We will disconnect anything that appears to be dangerous!

![A portable toilet Datenklo](/images/tumblr_inline_pdtbmgc9uL1rpuop0_500.jpg)

## Can you help?
We do need many hands for build-up. If you’re willing to come on Tuesday or Wednesday to help us build the network, please get in touch. Quick note to everyone reading this though: please do not arrive on site before Thursday 4pm if you haven’t [had a team leader confirm and sponsor your presence on site](https://www.emfcamp.org/about/volunteering#helping-with-setup-teardown), i.e. please don’t just turn up without an explicit invitation to do so. And [nobody should arrive before Tuesday](https://twitter.com/emfnoc/status/1031300067347574789).

We are also looking for people to join the team for the next event in 2020; in particular, we are looking for some people to help with systems administration. As this is a position of considerable trust, we need to get to know you first, so help out and introduce yourself this time around!

## They helped, many thanks

All these organisations have gone above and beyond to help us out preparing the network this time around, and without them it just wouldn’t have been possible to build the network we wanted to build. 

We thank:

![A list of sponsor logos](/images/tumblr_inline_pdtckaspO91rpuop0_500.png)

*Keep up with [@emfnoc on Twitter](https://twitter.com/emfnoc).*
