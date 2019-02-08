---
author: alexandre.normand
date: 2014-09-02 22:04:00-07:00
layout: post
Title: Glukloader 1.0-rc20 with Time Resolution Fixes and Growl Notifications.
---

The last week or so has been pretty interesting (see this [reddit post](http://www.reddit.com/r/diabetes/comments/2ei3qe/type_1_diabetic_and_software_engineer_i_thought_i/) for some details). The first few days showed how bad assumptions can quickly become blockers and then how other assumptions can manifest themselves in more subtle ways. 

## Time Resolution Bugs
I talked about the first blocker in the previous post but this is more about the latter. I had assumed that the Dexcom's internal time was standard. That is, I assumed that two receivers would have different display times but the same system time at any given point in time. That proved to be a bad assumption to make. [ChickenBeard](https://github.com/ChickenBeard) again helped with this bug by testing my numerous builds and being patient with my varied attemps at finding a more robust solution. 

I'm happy to say that it looks like my new approach is now working. The bad news is that previously uploaded data is bad and locally stored archives of your data (a copy that Glukloader keeps for you and for resending data in case of disasters) is also faulty (potentially). The result is bad times (it looks like bad timezone handling). It's not necessarily dramatic but I'd like to sanitize the data at some point. More to come as I think about this and talk to a few more of you to understand the impact. 

## Growl Notifications
Since Glukloader has proven to be very important to the whole interaction with Glukit, I decided to follow [edwhittle](http://www.reddit.com/user/edwhittle)'s suggestion and add some user feedback with it. 

## Download
Here's the link to the new build with both of those: [Glukloader 1.0-rc20](https://www.dropbox.com/s/7wjh03q9ch4sd87/glukloader%201.0-rc20.dmg?dl=1). 

Again, [talk to me](mailto:alexandre.normand@gmail.com) if there's anything on your mind.

Peace,
