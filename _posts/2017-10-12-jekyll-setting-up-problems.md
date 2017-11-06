---
layout: post
title: "Jekyll setting up problems"
date: 2017-10-12 15:13:24
categories: jekyll update
---
- running `jekyll s` returns `Permission Denied`
one possible reason is that in default `jekyll s` runs on the port 4000, which happen to be used by other program. Simply run `jekyll s --port 4001` to start,
or you can check out the available port by typing `netstat -a`(on windows).

- 
