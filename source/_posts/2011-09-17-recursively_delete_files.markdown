---
layout: post
title: "Recursively deleting a file"
date: 2011-09-17 17:50
comments: true
categories: [command line, osx, octopress]
---

I ran into a small bug in the latest pull from the octopress source.  It was complaining about .DS_Store files:

	➜  jcsims.me git:(master) rake deploy
	rake aborted!
	No such file or directory - public/_layouts/.DS_Store

	Tasks: TOP => deploy
	(See full trace by running task with --trace)

It's currently an [issue][1], but in the short-term I needed to remove all the pesky files from the project.
Enter this nice and easy command:

	find ./ -name \.DS_Store -ok rm {} \;

[1]: https://github.com/imathis/octopress/issues/150