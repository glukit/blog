---
author: alexandre.normand
date: 2014-08-25 21:01:03-07:00
layout: post
Title: Glukloader 1.0-rc11 now available.
---

Today was a big milestone for Glukit: someone else besides me used it. Or rather, someone else besides me tried to. 

Given the interesting and active discussions on [/r/diabetes](http://www.reddit.com/r/diabetes/), I had the intuition that I might find people who met my pretty strict requirements: Type 1 diabetic Dexcom G4 user with a Mac.

While this didn't go as smoothly as I would have hoped as people were giving it a spin, I was surprised to see this much activity on [my post](http://www.reddit.com/r/diabetes/comments/2ei3qe/type_1_diabetic_and_software_engineer_i_thought_i/). 

On the technical side, the biggest problem was due to a bad assumption (or oversight) I made a long time ago. Most people don't enter user events (injections, carbs) on their receiver and the receiver returns an indicator to say there's no data. Except I wasn't expecting such a value. With the logs kindly provided by [ChickenBeard](https://github.com/ChickenBeard), I was able to identify the bug and add tests to reproduce it. And [fix it](https://github.com/alexandre-normand/bloodSheltie/pull/22), too. 

So, for my fellow redditors that were kind enough to give it a try but experienced Glukloader becoming unresponsive, this might be an update that you want to try: [Glukloader 1.0-rc11](https://www.dropbox.com/s/b10xp67bgv635jc/glukloader%201.0-rc11.dmg?dl=1). 

Oh and there's also a timezone related bug that I'm trying to isolate at the moment. Hopefully, it won't be too long before I figure this one out.

Again, don't hesitate to [contact me]((mailto:alexandre.normand@mygluk.it).

Peace,