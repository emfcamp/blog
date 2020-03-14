---
layout: post
title: EMF Camp, the site and Networking
date: '2012-07-13T21:22:00+01:00'
tags: []
tumblr_url: http://blog.emfcamp.org/post/27143646219/emf-camp-the-site-and-networking
---
Provisioning high bandwidth connections is always fun, especially those that are only required for a very short period of time, and most notably, out in the middle of a field.

We’ve been very lucky to have [Pulsant](http://www.pulsant.com) sponsor us. They’re providing us with rackspace in both their Milton Keynes datacentre and in [Telehouse East](https://www.telehouse.net/) in London Docklands, giving us our own 1Gbps circuit between the two. Using this we’re constructing our own multihomed network, with multiple transit and peering connections, ensuring speedy Internet access for the entire camp.

Due to the 2.8km distance between the Pulsant data centre and Pineham Park, we’ll be erecting temporary 30 metre tall masts and creating a point-to-point microwave link to connect the camp. As you can see the masts are pretty impressive!

![A 30-metre tall mast](/images/2012_network_mast.jpg)

Here is a brief overview of what our core network will look like:

![Network Map](/images/2012_network_map.jpg)

Like all large hacking events in Europe (HAR2009/CCC) we’ll be using portaloos, or [datenklos](https://de.wikipedia.org/wiki/Datenklo), to house network switches and power distribution around the site. If you want super-fast wired access please make sure you bring a 40 to 50m Cat5 cable with you to connect your tent! (we are still finalising power plans and will post about these shortly).

![A portable toilet with network cables coming out of the door](/images/6045763700_7b870a56e2_d.jpg)

(credit binarycoco)

[Chaos Computer Club](https://en.wikipedia.org/wiki/Chaos_Computer_Club) in Germany are lending us their event IP address space, so everyone at the camp will get a real public IP. At the moment we’re working on configuring the core network, wireless controllers and various services (DNS, DHCP, monitoring etc).

![Stacks of network switches and access points](/images/2012_network_equipment.jpg)

[flexOptix](https://www.flexoptix.net) have sent us the first shipment of loan optics, we’ll be using these to building multiple rings around the site, linking venues and dateklos.

![Optics and Flexbox programmer](/images/2012_network_optics.jpg)

At the site we will have blanket wireless coverage on 2.4GHz (b/g/n) and 5GHz (a). If you have any particular network requirements, or if you plan to use any non-Wifi devices in these frequency bands, please let us know in advance at noc@emfcamp.org

Finally, a big thanks to [Nick Ryce](https://twitter.com/netdonkey) and Matt Lovell at Pulsant for providing the rackspace and circuit between London and MK, CCC for use of their address space, and flexOptix for loan of their SFP optics.
