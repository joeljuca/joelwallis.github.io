---
published: true
layout: post
title:  "Quick and safe random passwords"
permalink: random-passwords.html
date: 2017-01-23T17:00:00.000Z
tags: security
---

Have you ever needed to quickly generate a new password, e.g., for some service
you were signing in - or whatever else?
Well, here's a quick and dirty way to generate safe passwords direct from
the command line:

```
$ head /dev/random | md5
```

It will quickly generate you a 32-char password direct from your operating
system's [random number generator][dev-random].
For those not used to `/dev/random`, it's a special file that has only random
content, collected from input devices and other sources (more info at the
[Wikipedia page about `/dev/random`][dev-random]).

One possible alternative that can generate you a 40-char password is to use
`shasum` instead of `md5`:

```
$ head /dev/random | shasum
```

Cheers!

--  
_PS: `md5` and `shasum` are commands available in OS X/macOS. If you use Linux or
BSD they may vary. Please check your OS documentation for more info about
hashing utilities/commands for your command line._

[dev-random]: https://en.wikipedia.org/wiki//dev/random