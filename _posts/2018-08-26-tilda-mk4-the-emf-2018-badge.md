---
layout: post
title: TiLDA Mk4, The EMF 2018 badge
date: '2018-08-26T22:30:16+01:00'
tags: []
tumblr_url: http://blog.emfcamp.org/post/177423823788/tilda-mk4-the-emf-2018-badge
---
Electromagnetic Field 2018, the event that celebrates technology, science, engineering, and weird inventions, is just around the corner again. And [like](http://blog.emfcamp.org/post/28558155390/revealing-tilda-our-camp-badge) [previous](http://blog.emfcamp.org/post/94157161753/announcing-tilda-mke-the-incredible-emf-2014-camp) [years](http://blog.emfcamp.org/post/145667126793/the-emf-tilda-badge-is-saved) we have a free ready-to-hack electronic badge for all attendees.

We’ve gone all out this year, doing things that many said were impossible. You might have seen our [previous blog](http://blog.emfcamp.org/post/176799817383/bring-out-your-dect) about the experimental GSM mobile phone network we’re deploying - but did you guess that we built it for the badge?

Thanks to the generous sponsorship and support provided by [Texas Instruments](https://ti.com), [HCD](http://www.hcduk.com), [Seeed Studio](https://www.seeedstudio.com/) and the hard work of our Badge Team we’ve topped all previous versions - say hello to the TiLDA Mk4.

![The TiLDA Mk4 badge](/images/tumblr_inline_pe2zdsGuvv1rpuop0_500.jpg)

## Call me maybe?
The astute among you will notice the keypad, call, and end buttons on the badge. That’s because we took inspiration from the old [Nokia N-Gage](https://en.wikipedia.org/wiki/N-Gage_(device)) - every single badge is a fully-functioning fully-hackable python-powered mobile phone!

An on-board SIM800 GSM module allows you to make & receive calls, send text messages, and use data anywhere in the world. At camp it’s a fun toy, but when you leave it’s perfect for remote IoT connectivity.

In order to support this the [POC team](http://blog.emfcamp.org/post/176799817383/bring-out-your-dect) have built a fully-licensed GSM network, in cooperation with [Lime Microsystems](https://limemicro.com/news/lime-provides-limesdr-mini-and-raspberry-pi-base-stations-for-emf-camp/) - this is the year where EMF becomes a mobile phone network operator!

Each badge comes equipped with a SIM card, thanks to [Hologram](https://hologram.io). These sims work with the on-site network for voice and SMS, and when you leave camp they’ll work as IoT data SIM cards anywhere in the world.

## There’s a Badge App for that
We have a Badge Store that allows everyone to easily install apps other attendees created. So if you want to do something fun with the TiLDA Mk4 start planning now!

In the spirit of collaboration, we want to encourage everyone to see if they can improve on [any of it](https://github.com/emfcamp/Mk4-Apps) and send us loads of [pull requests](https://help.github.com/articles/about-pull-requests/) - before, during or after the event!

Keep an eye on [https://badge.emfcamp.org/2018](https://badge.emfcamp.org/2018) - we’re hoping to get some documentation there soon. You can also [join us via IRC on freenode in #tilda](https://www.irccloud.com/invite?channel=%23tilda&hostname=irc.freenode.net&port=6697&ssl=1).

## Hack it
TiLDA Mk4 uses TI’s latest [SimpleLink MCU Platform](http://www.ti.com/wireless-connectivity/simplelink-solutions/overview/overview.html) running the most up-to-date version of [MicroPython](https://micropython.org/), which means you can program your badge as easily as copying text files to a usb stick.

We want every attendee to make improvements to their own badge and share them with others. To that end we will run workshops, provide space to work and hands-on help in our dedicated badge tent. Just make sure you’re bringing your laptop if you want to take part!

We’re still furiously coding to prepare for your arrival in the field, but if you can’t wait to see what we’re up to, check out the [repository](https://github.com/emfcamp/Mk4-Apps). We’re trying to provide a set of [useful libraries](https://github.com/emfcamp/Mk4-Apps/tree/master/lib) to make it easier to get started. 

If you want to hit the ground running and you happen to have an EMF 2016 badge, you can refresh your MicroPython skills with that - we’re aiming to make porting existing apps to the TiLDA Mk4 as easy as possible, but expect to do some adapting once you get the final hardware.

![The rear of the TiLDA Mk4](/images/tumblr_inline_pe2zn8aFAp1rpuop0_500.jpg)

This year’s hardware includes:

* Texas Instruments [MSP433E4 SimpleLink Microcontroller](http://www.ti.com/product/MSP432E401Y) (ARM Cortex-M4F @ 120MHz)
* Texas Instruments [CC3120 SimpleLink Wi-Fi® Network Processor](http://www.ti.com/product/CC3120)
* 256KB internal RAM / 8MB external SDRAM
* 1MB internal flash (firmware) / 1MB external flash (filesystem)
* [SIM800](https://simcom.ee/documents/SIM800/SIM800_Hardware%20Design_V1.08.pdf) Quad-band GSM/GPRS module with Bluetooth support
* 240x320 [RGB screen](https://cdn.hackaday.io/files/11178478239552/ER-TFT024-3_Datasheet.pdf)
* 2 [WS2812B](https://cdn-shop.adafruit.com/datasheets/WS2812B.pdf) RGB LEDs (aka Neopixels) with a 3-pin header to connect your own (And this year they’re the right way up!)
* Texas Instruments [HDC2080 Low Power Humidity and Temperature Sensor](http://www.ti.com/lit/ds/symlink/hdc2080.pdf)
* Texas Instruments [TMP102 Digital Temperature Sensor](http://www.ti.com/lit/ds/symlink/tmp102.pdf)
* Texas Instruments [OPT3001 Digital Ambient Light Sensor](http://www.ti.com/lit/ds/symlink/opt3001.pdf)
* Texas Instruments [DRV5055 High Accuracy Bipolar Hall Effect Sensor](http://www.ti.com/lit/ds/symlink/drv5055.pdf)
* Speaker and Microphone
* 2000mAh Battery
* Onboard Ethernet (requires breakout)
* A [T9](https://en.wikipedia.org/wiki/T9_(predictive_text)) number keypad and a joystick
* 2 [Seeed Studio Grove headers](http://wiki.seeedstudio.com/Grove_System/) (one [UART](https://en.wikipedia.org/wiki/Universal_asynchronous_receiver-transmitter), one [I²C](https://en.wikipedia.org/wiki/I%C2%B2C))
* [Conductive thread](https://learn.sparkfun.com/tutorials/sewing-with-conductive-thread) points and 0.1" header for power/UART/I2C/GPIO
* [Defcon 26 Shitty Add-Ons connector](https://hackaday.io/project/52950-shitty-add-ons)

## Badge competition
Finally, we would like to congratulate last year’s [winner of the badge competition](https://twitter.com/floppy) for his amazing 3D renderer. We’re going to run the competition again this year and we can’t wait to see what you come up with.

Here’s some ideas for things to experiment with:

* A synthesiser using the built-in speaker, and bluetooth
* Using the on-board ethernet to connect to the network
* An IoT monitoring package, for remotely reporting the on-board sensors
* Controlling hardware & installations via SMS messages
* Geolocation using cell tower information
* DTMF detection, for “press one to turn on the giant laser”
* Voice synthesis, for talking to incoming callers
