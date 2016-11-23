---
published: true
layout: post
title:  "Trying out CyanogenMod"
permalink: trying-out-cyanogenmod.html
date: 2016-11-23T12:00:00.000Z
tags: android cyanogenmod
---

I'm now using an old [Moto G 2014 (2º gen)](https://en.wikipedia.org/wiki/Moto_G_(2nd_generation)) now after destroying my old [LG Nexus 4](https://en.wikipedia.org/wiki/Nexus_4). My smartphone needs are pretty simple: I don't do gaming on it, just calling, messaging and some office-related stuff (email, calendar, auth tokens, etc.). A basic one like Moto G could get the job done, right?

Well, my problem was the poor performance I was getting from this Moto G. It comes with lots of apps installed by default on its Android, running without being used. So yeah, I was not happy with it at all, and I started to think about acquiring a new one. [Moto G4 Plus](https://en.wikipedia.org/wiki/Moto_G4) came into mind, but a friend suggested [CyanogenMod](https://www.cyanogenmod.org) and I decided to give it a try.

## First things first: backup your stuff

Most of my things are kept in sync: data are generally synced to Drive or Dropbox, and photos and videos are uploaded to Flickr, so it was quite easy for me to proceed from this step, but **you must make sure you backing up your data, otherwise you will lose it forever.**

## Install Android SDK

if you're on a Apple device (Mac, MacBook, etc.), installing it with [Homebrew](http://brew.sh) is quite easy.

    $ brew install android-platform-tools

You can find additional 

## Acquire root-level permissions

TODO: explain rooting steps.

## Install CyanogenMod

**DISCLAIMER: The following informations may lead your smartphone to a unusable state - it means you can "brick" it. I take no responsibility for such cases, so proceed at your own risk.**

I faced some serious issues while installing CyanogenMod (from now I'll just use CM as its abbreviation) for the first time, so I'll state here some important infos before proceeding:

1. **Your smartphone does not charge well when in fastboot mode**  
   [fastboot](https://wiki.cyanogenmod.org/w/Doc:_fastboot_intro#A_brief_introduction_to_fastboot) is an advanced way to realize very basic operations, like [flashing](https://wiki.cyanogenmod.org/w/Basic_concepts#.22flashing.22) a partition (equivent to formatting a PC hard drive), so make sure your smartphone battery is at 100% before starting the process.
1. **Don't do multitasking while doing the install operation**  
   That was my mistake. I started with my smartphone battery at full capacity, but I was multitasking during the process. Result? I took so much time to research, understand, learn and apply every single step that my battery lose all of its power and suddenly everything became much harder than it needed to be.
1. **Understand the process before starting it**  
   Or at least most of it. I spent much more time reading and understand the process than I spent installing the CM, so read stuff before starting the process.
1. **Don't format your smartphone's partitions until you've downloaded everything and is ready to proceed**  
   You'll need a recovery image (I used the Team Win Recovery Project)

### Replace your smartphone recovery image