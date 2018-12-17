---
layout: post
title: 'How to network a field: Internet-to-the-tent at EMF 2014'
date: '2014-08-18T11:19:00+01:00'
tags: []
tumblr_url: http://blog.emfcamp.org/post/95086800438/how-to-network-a-field-internet-to-the-tent-at
---
Delivering a reliable high-speed wired and wireless network to a campsite in just over two days is something of a challenge. Fortunately, [the NOC team](https://wiki.emfcamp.org/wiki/Team:NOC) is filled with people who have done just that year after year at events across Europe and the world. The network this year is based on those experiences and on our work at EMF 2012.

This is the first of two blog posts we’ll be releasing about the network setup. Here, we’ll talk about the on-site network. Next time we’ll talk about our uplink and connections to the Internet. 

Let’s start with where the network connects to you, the camper.

## Wired Network
![A portable toilet with wires coming out](/images/tumblr_inline_p8ne7kTHmI1rpuop0_500.jpg)

Despite all available evidence, this is not a public toilet. This is a Datenklo (German: “data toilet”), or DK for short. We use them as distribution points for network and power across the field, because they are conveniently-sized lockable containers, provide protection against the weather, and are relatively cheap to hire.

![A lot of power sockets inside a portable toilet](/images/tumblr_inline_p8ne7kRYcl1rpuop0_500.jpg)

Inside each DK is a power distribution box with circuit breakers, one or two network switches, and a wireless access point. Often they come with a free roll of toilet paper.

We expect all camping areas to be within 50m of a Datenklo. Most are closer, but we recommend you bring up to 50m of Cat5 cable if you want to connect to your tent. Likewise, if you want power, it is best to bring a long cable (although it is likely that there will be closer distribution points around the field if you instead bring a 16A commando connector).

Just leave your cables in an obvious position outside the door so we can see them, and someone will be around to connect them up regularly. If this doesn’t happen quickly enough, you can follow the instructions on the DK to tweet or SMS us.

Note that, to prevent inadvertent network loops, port-security is enabled on all edge ports. So you won’t be able to connect more than one device to a port. If you want to connect a switch, come and talk to us on-site in the NOC and, as long as you sound like you know what you’re doing, we’ll raise the restriction on your port.

## Distribution and Core
![A network diagram](/images/tumblr_inline_p8ne7kNu881rpuop0_500.png)

This year we’re anticipating much higher bandwidth usage, so our network architecture has grown to suit. DKs will be cabled back, using fibre or Cat5e, to one of three distribution switches acting as aggregation points, located around the field in DKs. Each will take the Gigabit Ethernet port-channels from 8-12 DKs each and aggregate them into 10-Gigabit Ethernet uplinks into the core.

The CCC have lent us their reels of outdoor fibre, which are allowing us a much more scalable network design over a larger area. FlexOptix are kindly loaning us all the optics to plug into the switches. The fibre SFPs are something akin to magic: they use different frequencies in each direction to allow bidirectional communication down a single core of fibre.

## Wireless
The other thing inside (or possibly on top of) a DK is the wireless access point. We aim to provide seamless wireless coverage and roaming across the entire field including all the camping areas. Thanks to the sponsorship of Aruba Networks, we’ll be deploying their access points across the field, all tunnelled back over the wired network to a centralised 7210 controller in the NOC that will handle authentication and roaming. So even if you walk from one end of the field to the other, your IP address will not change and your connection should be seamless. In some places you’ll even be able to get a 802.11ac gigabit-speed wireless connection.

In a departure from the norm, this year the main wireless network will be using WPA2-Enterprise. This ensures that everyone gets their own key and are safer from snooping. We still recommend using end-to-end encryption, but this will help protect you. To connect to the network, join the “emfcamp” network and use the username “emf” with password “emf”.

If your device doesn’t support 5GHz, you can join the legacy network “emfcamp-legacy”, but be aware that this is less resistant to interference and will be less reliable. Use the other one if possible.
For those really old devices that don’t even support WPA2-Enterprise, there’s a network called “emfcamp-insecure”. Please don’t use this unless you really have to.

## How can you help?
![A picture of network diagrams](/images/tumblr_inline_p8ne7lWxLB1rpuop0_500.jpg)

The NOC team is always a popular one, but we don’t really need any help during the event. By Friday morning, the network should be up and running perfectly and we’ll be putting our feet up! What we do need help with is setup and teardown. During setup, there are a LOT of cables to run (at least 5km worth), RJ45 plugs to crimp, and switches to deploy, and then the whole lot needs to be collected up at the end. At the moment, we’re looking fairly good for setup, but we need more help for teardown.

If you’re interested, please drop a line to noc@emfcamp.org letting us know when you can arrive and when you have to leave. You’ll even get fed!

## More information
There’s more information on how to use the network, including a few “do"s and "don’t"s, on our wiki page.
Have a question? Drop us a line at noc@emfcamp.org or follow us on twitter.

## Sponsors
We are grateful to our sponsors Comtec who are providing the access and core switches and routers, LONAP who are providing the Summit x650 distribution switches, Aruba Networks who are providing the access points and wireless LAN controller, and FlexOptix who are providing the necessary optics to link it all together.

