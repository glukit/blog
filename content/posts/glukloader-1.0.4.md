---
author: alexandre.normand
date: 2015-09-27 22:00:00-07:00
layout: post
Title: Glukloader 1.0.4
---

Here's a bugfix release for something I hope I was the only one experiencing. I had noticed that my keyboard and mouse (and USB peripherals) on `iMac` would sometime stop working after it going to sleep. At first, I suspected a hardware issue but I started noticing one day that I had my Dexcom receiver plugged in before my Mac went idle. And it happened a few more times when my receiver was plugged in again. So I cleaned up a little the management of the USB device and made sure it would be closed after a successful sync rather than keeping it open. After some testing, it looks like that might have been it. 

Or maybe it was all a coincidence but either way, `Glukloader 1.0.4` is being a little more conservative in closing the resources and it's for the best.

If you did have mysterious issues with your peripherals not responding after going idle, I apologize. Hopefully, this will solve that mystery. 

Grab the latest build [here](https://dl.dropboxusercontent.com/u/3208429/glukloader%201.0.4.dmg?dl=1).
