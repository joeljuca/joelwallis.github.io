---
published: true
layout: post
title:  "Integration tests and CI"
permalink: travis-and-sensitive-logs.html
tags: node.js travis testing security
---

I recently built a very simple API that will be used by one of my students.
It uses both [Google Maps API](https://developers.google.com/maps/) and
[SunsetWx API](https://sunburst.sunsetwx.com/v1/docs/) to predict the quality of
sunrise and sunset for a given address (recognizable by Google Maps, of course).
I used the opportunity to practice testing, since I didn't have many
opportunities to work on projects with automated tests during my career.
As a newbie in the field, I tried to follow some of the best practices I've been
reading about, and I really liked the
[final result](https://github.com/joelwallis/thinkful-sunset-backend). 😃

Writing the unit tests was quite easy. It was not my first time writing unit
tests, I've contributed to [Exercism](http://exercism.io) before, with code that
included unit tests
([exercism/javascript#372](https://github.com/exercism/javascript/pull/372)).

Turned Travis CI on, pushed my local commits to `master` and watched my logs.

But I also included integration tests on my test suite, which are basically API
calls using provided credentials. However, I didn't wanted to have these
credentials being shown in Travis

Integration tests took me an additional time to figure how I should have been
writing them, and in the end I just added them as additional test cases
(suggestions are more than welcome).
