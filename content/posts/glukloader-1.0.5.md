---
author: alexandre.normand
date: 2015-10-05 21:00:00-07:00
layout: post
Title: Glukloader 1.0.5
---

Just after `Glukloader 1.0.4`, I upgraded to `El Capitan` (OS X 10.11) to find that `Glukloader` wasn't working anymore (not synching). 
It seems that the behavior regarding an internal event changed in 10.11. I found an alternative and that's what's new in `Glukloader 1.0.5`. I also reverted
a change from `1.0.4` to try and address instability issues when the receiver was plugged in on a Mac going idle. After some reading, I realized that this
is something that [ORSSerialPort](https://github.com/armadsen/ORSSerialPort) was supposed to be handling gracefully so I decided to upgrade to the latest 
release (which has a few related fixes) and see where this would get me.

So, if you see this bug with `1.0.5`, please contact me. 

Grab the latest build [here](https://www.dropbox.com/s/5jr8wrgq5bmspbx/glukloader%201.0.5.dmg?dl=1).
