---
published: true
layout: post
title:  "Creating a GNU/Linux bootable USB from OS X/macOS"
permalink: bootable-usb.html
date: 2017-06-25T21:00:00.000Z
---

I'm always in need to create bootable USB sticks to try and/or install a Linux
distro somewhere - generally, Debian/Ubuntu based distros. So, to avoid
_googling_ how to do it every time, here's the instructions:

**First, convert the `*.iso` file to `*.img`**  

```
hdiutil convert your-file.iso -format UDRW -o your-file.img
```

_Note: OS X tends to put the .dmg ending on the output file automatically._

**Then, find out your device address**

You device address will look like `/dev/diskX` - being X a number (e.g.:
`/dev/disk2`).
Run `diskutil list` and try to figure which one is your USB stick.

If you're still unsure about your device address eject your USB stick, run
`diskutil list` and save the output.
Then, insert your USB stick, run `diskutil list` again and compare the outputs.
