---
author: alexandre.normand
date: 2014-09-18 21:01:00-07:00
layout: post
Title: ♥ mmol/L
---

Glukit had been built with multiple glucose units in mind but, to minimize the scope of the initial testing, the front-end had been made to support only mg/dL. I'm happy to say that this is now no longer the case. If your Dexcom is set to mmol/L, you'll now be able to browse your data in the unit you're used to. 

#### Glukloader Required Upgrade
In the troubleshooting process with a friend from UK, I found a critical bug in my interpretation of the glucose values when the unit was mmol/L. If you're a mmol user, you need to upgrade to the most recent build to get proper values: [Glukloader 1.0-rc23](https://www.dropbox.com/s/5vrtaofgx4curih/glukloader%201.0-rc23.dmg?dl=1). You should also [drop me a line](mailto:alexandre.normand@mygluk.it) so we can reset your data uploaded with previous versions. 

The build also includes a handy new feature: emailing glukit logs with a simple one-click action (in the "Advanced" menu).

Peace,
