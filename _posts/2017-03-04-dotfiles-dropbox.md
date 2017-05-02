---
published: true
layout: post
title:  "Using tmuxinator? Backup your tmux setups with Dropbox"
permalink: tmuxinator-dropbox.html
date: 2017-03-05T00:00:00.000Z
tags: dotfiles
---

It's a quick and easy way to backup your tmuxinator-powered tmux setups. Just
move the `~/.tmuxinator` folder to your Dropbox and voilà! :-)

Here's how you can do it (assuming that your Dropbox files are located in your
home directory - so its path is `~/Dropbox`):

```
cd ~
mkdir Dropbox/tmuxinator
mv .tmuxinator/* Dropbox/tmuxinator
ln -fs Dropbox/tmuxinator .tmuxinator
```

_PS: you can also use Google Drive, OneDrive or any other cloud-based storage
solution._
