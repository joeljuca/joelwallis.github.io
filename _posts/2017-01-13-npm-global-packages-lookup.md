---
published: true
layout: post
title:  "Checking npm global packages"
permalink: npm-global-packages.html
date: 2017-01-13T13:00:00.000Z
tags: nodejs npm
---

I recently needed to check which packages I had installed globally.
In my very specific need, I was intended to uninstall
[Yarn](https://yarnpkg.com/)'s npm package to then be able to install it through
[Homebrew](http://brew.sh/), which is the recommended way for OS X/macOS.

I then needed to first check if it was installed globally on my local npm, but
after running `npm ls -g` I got a reeeally big output with packages,
dependencies and recursive dependencies' dependencies, etc., so... :'(

BUT, turns out that it's quite simple to solve:

```bash
npm ls -g --depth=0
```

The flag `--depth=0` ensures that only top level packages (which are the ones
you might be more interested on) will be listed. Yay!
