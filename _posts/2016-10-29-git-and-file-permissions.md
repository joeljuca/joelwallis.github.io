---
published: true
layout: post
title:  "Stop versioning file permissions with Git"
permalink: file-permissions-and-git.html
date: 2016-10-29T17:00:00.000Z
tags: git
---

**Just do it. Don't even dare asking, just do it.**

_[Bhreathes heavily...]_

OK then, I'll explain one more time. A [D]VCS like Git enables asynchronous but
still very organized developer contributions, and that's it.
Setting up the file system and its permissions, etc., is part of the deployment
process, and thus, a responsibility for its automation.
When you allow Git to mess your project's file permissions scheme god kills a
kitten and you can be sure you'll be accounted for.

Enough talking. Now, from your repository folder, run:

```
git config core.fileMode false
```

Also, please make it a global config:

```
git config --global core.fileMode false
```

Thank you very much.
