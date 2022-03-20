---
layout: post
title: "Raspberry PI USB issues - it's probably not the software's fault"
categories: raspberry
---

#### Raspberry pi USB devices just not working? Are they seen by the pi, yet refuse to do basic functions? Then this article might help you

Recently, I was trying to do a Raspberry project - a tiny travel router. I had both a USB Wifi dongle and an external LTE modem, and both refused to work.
They were detected correctly by the driver, but just didn't connect. I thought it was an OpenWRT issue, but it's much simpler than that.  
Raspberry Pi USB ports just give too little power output. At first I thought "Well my tiny wifi dongle definietly does not take that much power!". But after some experimenting, I found the core issue.

#### Solution

Use a Powered USB HUB. The HUB needs to have a separate port for power and data. Connect the power port to the plug directly, and the data to the Pi.  
This isn't the cleanest soluton. It leaves a mess of cables. I'm working on improving this to make it more portable, but just know the core issue is USB power.

#### Thanks for reading
