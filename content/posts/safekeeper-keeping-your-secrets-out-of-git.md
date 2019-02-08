---
author: alexandre.normand
date: 2015-02-22 10:00:00-07:00
layout: post
Title: Safekeeper, Keeping Your Go Secrets Out of Git
---

I've been wanting to open-source [Glukit](https://mygluk.it/) for a while but I had to find a way to keep the client ids/secrets safe and outside of git before I could do so. 

Since Glukit runs on the Google App Engine, it can't itself just read the sensitive information from environment variables. I read a post that [suggested storing the secret keys in the datastore](http://pseudony.ms/blags/secret-keys-gae.html) but I had quite a few and felt like this solution lacked good integration in the development flow. 

After reading about [go generate](http://blog.golang.org/generate), I thought that this might be a good use for it. If I could get a way to use [go generate](http://blog.golang.org/generate) and generate my app secrets into code that was going to be ommitted from the repository, I'd have something relatively simple and convenient. 

### Enter safekeeper
Based on the [go generate](http://blog.golang.org/generate) examples, I set myself out to create a command-line tool that would take a few inputs and generate a file to be git ignored containing all application secrets. You have to [follow the instructions](https://github.com/alexandre-normand/safekeeper/blob/master/README.md) to get a nice integration but once it's set up, developers can set their secrets in their environment and then they just have to run `go generate` or `goapp generate` to get them into the code to deploy or run. 

I tried to include a detailed example of how it can be used effectively but [let me know](mailto:alexandre.normand@gmail.com) if you find anything missing.

Cheers!

