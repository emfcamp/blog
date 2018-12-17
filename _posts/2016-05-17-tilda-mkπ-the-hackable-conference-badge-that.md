---
layout: post
title: 'TiLDA Mkπ: The Hackable Conference Badge That Needs Your Help'
date: '2016-05-17T20:18:06+01:00'
tags: []
tumblr_url: http://blog.emfcamp.org/post/144514906298/tilda-mkπ-the-hackable-conference-badge-that
---
## Short version:

If we don’t secure additional sponsors in the next two weeks, we will be forced to cancel the EMF 2016 badge.

## Long version:

[Electromagnetic Field](https://www.emfcamp.org) is a UK festival celebrating technology, science, engineering, and weird inventions. At each of our events so far, we’ve given out a hackable electronic badge for free to all attendees. 

We always aim high, and until this year we’ve managed to pull it off with the help of an array of lovely sponsors. The TiLDA badge is entirely funded through sponsorship; we are committed to keeping our ticket prices as low as possible.

For EMF 2016, we set two goals: **Python**, and **WiFi**. Real WiFi on each of our 1700 attendees’ conference badges.

After months of work, we have a final design and we’re ready to go into production. We have sponsorship for all the major components, covering the majority of the cost of the badge, but despite heroic efforts, we haven’t managed to find a sponsor to support the PCB fabrication and assembly of the badge.

We have two weeks left in our schedule before we must start building badges. If we haven’t secured sponsorship by then – we need about £15,000 or a friendly manufacturer to sponsor it in-kind – we’ll have no option but to cancel the project entirely.

**If you know of anyone who may be willing to help, we’d urgently like to hear from them.**

## What is the TiLDA Mkπ?

Thanks to the very generous sponsorship of [STMicroelectronics](https://st.com) and [Texas Instruments](https://ti.com) we’ve spent the last year designing, testing and programming a badge that both runs Python and is WiFi-enabled.

![A prototype badge](/images/tumblr_inline_o7dh6n90Iw1rpuop0_500.jpg)

*(Images in this post are of working development prototypes - the production version will feature better artwork and a less offensive PCB colour.)*

The TiLDA Mkπ has ST’s newest full-featured, ultra-low-power 80MHz **STM32L4 microcontroller**, a **TI CC3100 WiFi module**, a **large colour screen**, **gyro** and **magnetometer** from ST, many other inputs and outputs, a **MicroSD card slot**, and a **large rechargeable battery**. Of course, it also features a blindingly bright **RGB LED** for the ever-popular “torch mode”, and simple connections to attach wearable devices.

On top of this, TiLDA runs [Micropython](http://micropython.org/), which makes showing your name on the screen a simple `print('Dave’)`, and activating the torch is just `led.high()`.

Plug the badge into your computer using USB, and programming it is as easy as editing a Python file on a drive. We also hope to make it possible to write code in your web browser over WiFi.

At EMF, we plan to have a full set of software already loaded and the ability to wirelessly install new apps. We want the TiLDA to give experienced attendees the easiest possible way to build internet connected devices, while being a brilliant teaching tool for those who are just starting out.

![The rear of the badge](/images/tumblr_inline_o7dh5yjFI61rpuop0_500.jpg)

The entire design is open source, and we hope that people will improve the design and code to develop amazing new things.

## Who is sponsoring?

Texas Instruments and STMicroelectronics have been extremely generous, committing to supply the major components for the badge, helping us develop the Micropython WiFi driver, and introducing us to other potential partners. We’re indebted to them for their support.

## What we need

**In two weeks we will hit supply deadlines for some of the badge components and we have to make a decision about continuing the project.** EMF is a non-profit, volunteer-run organisation and we can’t take a financial risk on the badge without endangering the whole event.

Before then we either need to secure enough money to pay for manufacture from one or more sponsors, or find a PCB assembly company who are willing to sponsor.

## I would like to help!

You can email us on badge@emfcamp.org, or you can call us on +44 (0)1908 870 919 (9am-5pm BST, Monday to Friday).

For more information about sponsoring EMF, [visit our sponsorship page](https://www.emfcamp.org/sponsor).

## What if nobody sponsors?

Today we’re [open-sourcing the design](https://github.com/emfcamp/Mk3-Hardware) of the badge and we’re in the process of integrating the WiFi driver into Micropython. We hope that others will take our work and run with it.

![PCB traces on the badge](/images/tumblr_inline_o7cbcfUgzo1rpuop0_500.png)

EMF 2016 will continue regardless, and it will still be awesome even if we can’t build the badge. If this post has made you curious, tickets will be back on sale around the beginning of June.

After EMF is over, we may take orders for a small batch of the badges for anybody who wants one - keep an eye on our twitter account and this blog for updates!

Whatever happens, you can be sure that our presentation about the badge at EMF will be full of drama.

## Who did all this?

We’d like to thank Matt Brejza, Bob Clough, Kimball Johnson, and Matt Lloyd for their tireless work and late nights over the last year. We’d also like to thank Damien George for writing Micropython.
