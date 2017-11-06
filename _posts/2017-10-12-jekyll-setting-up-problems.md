---
layout: post
title: "Jekyll setting up problems"
date: 2017-10-12 15:13:24
categories: jekyll update
---
- running `jekyll s` returns `Permission Denied`
one possible reason is that in default `jekyll s` runs on the port 4000, which happen to be used by other program. Simply run `jekyll s --port 4001` to start,
or you can check out the available port by typing `netstat -a`(on windows).

- When running jekyll in a newer version, the dependent libs are somehow not working any more.Some said try `bundle cleanup`, which in my case is not working.I follow the suggestion, delete the `Gemfile` and `Gemfile.lock`, problem solved.And another warning shows up, `Deprecation: The 'gems' configuration option has been renamed to 'plugins'. Please update your config file accordingly.`, just rename the `gems` in `_config.yml` to `plugins`.
