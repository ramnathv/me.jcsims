---
date: 2011-07-08 17:52
layout: post
comments: true
categories: [mac, osx, terminal]
title: "Unhide Library In Lion"
---

For those of you who may have the benefit of already using Mac OSX Lion (or those of you who will be using it in the next two weeks), you may notice that the Library folder is now hidden in your home directory.  Luckily, there's an easy fix:

	chflags nohidden /Users/<Username>/Library

This was overwritten after upgrading between dev releases of Lion, so we may see this same issue continue in Lion.