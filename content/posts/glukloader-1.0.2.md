---
author: alexandre.normand
date: 2015-01-12 10:00:00-07:00
layout: post
Title: Glukloader 1.0.2
---

I got a log file in my inbox earlier this evening. Sometimes, people write an accompanying email describing a problem but this time, I only had the log file. It didn't take long to see the crash and stack trace in the logs. After a quick investigation, I found that there was a bug when the last sync had been done long enough ago that the last page synched didn't exist anymore on the receiver. That was an easy fix and I just pushed the release with the bugfix. 


Grab the latest build [here](https://dl.dropboxusercontent.com/u/3208429/glukloader%201.0.2.dmg?dl=1).

Thanks to the anonymous bug report!
