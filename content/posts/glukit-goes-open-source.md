---
author: alexandre.normand
date: 2015-02-22 10:30:00-07:00
layout: post
Title: Glukit Goes Open-Source
---

I'm happy to announce that I finally decided to fully open-source Glukit, Glukloader and glukameleon (a little tool used in dev) under the [MIT license](https://github.com/alexandre-normand/glukit). The main blocker was that I needed to find a solution to keeping client ids and client secrets outside of the repository and I [found something I'm happy with now](/posts/safekeeper-keeping-your-secrets-out-of-git).

I was hesitant to open-source Glukit for a while because much of its value resides in the centralized service that enables you to be compared to other diabetics. It's a bet but I'm hoping that Glukit going open-source won't mean everyone starting their own instance. And even if that happens, that might not be the end of the world. 

Here are where the repositories can be found:

* [Glukit](http://www.mygluk.it/), the main app, written in Go: [https://github.com/alexandre-normand/glukit](https://github.com/alexandre-normand/glukit).

* [Glukloader](https://github.com/alexandre-normand/glukloader), the OS X uploader, written in Objective-C: [https://github.com/alexandre-normand/glukloader](https://github.com/alexandre-normand/glukloader).

* [glukameleon](https://github.com/alexandre-normand/glukameleon), a command-line tool to convert Dexcom Studio XML files into json files understood by glukit, written in Go: [https://github.com/alexandre-normand/glukameleon](https://github.com/alexandre-normand/glukameleon).

* [safekeeper](https://github.com/alexandre-normand/safekeeper), a command-line tool to use with [go:generate](http://blog.golang.org/generate) to keep secrets safe from the git history by generating code from environment variables, written in Go: [https://github.com/alexandre-normand/safekeeper](https://github.com/alexandre-normand/safekeeper).

If you decide to grab the code and try hacking and find yourself lost, don't hesitate to [get in touch](mailto:alexandre.normand@mygluk.it).

Cheers!

