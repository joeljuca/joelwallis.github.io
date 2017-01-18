---
published: true
layout: post
title:  "The DOM of JavaScript"
permalink: javascript-dom.html
tags: javascript
---

_Or, why you'll hear that JavaScript sucks as hell very often._

If you are joining the JavaScript world you will hear people saying terrible
things about JS, from the well stated _"JS is a badly architected language"_,
_"JS doesn't even have a standard library"_ and _"JS turn complex simple
things"_, to the more general _"JS sucks!"_ or _"JS is the worst thing in web
development"_, etc.
This article will try to make you understand a bit more about this phenomenom.

## Once upon a time, there were JavaScript

JavaScript was made in 95 to provide the ability to manipulate web pages and
save some back-end processing.
Yeah, it was initially made for laypeople.
Then, with the advent of Ajax, and more recently CommonJS, it received a lot of
attention from serious/professional developers.
But, how was it possible to develop such big software project with a language
that even lacks a proper standard library, module system, package management,
task automation, linting, etc., etc. - plus all kinds of best practices to work
with it?

OK, you got the scenario.
The community was already moving fast at this time, but setting up standards for
JavaScript was not a simple task: it was an object oriented language but had no
classes; it allowed you to share functionality between objects/instances but
through prototype chains instead of class hierarchies; functions were first
class citizens, being even treated like data structures... But nobody were
gaving a fuck to it!

People wanted to code JS the same way they were coding PHP, Ruby, Python, etc. -
so the first frameworks bringing those solutions started to arise.
I remember [Prototype][prototype-www], [script.aculo.us][scriptaculous-www] and
[Dojo][dojo-www] from mind, but there were many others, trying to ease the pain
of working with JavaScript.
Even [jQuery][jquery-www] were released the same period, and  all kinds 
practices arose together - not really best practices, and some of them not even
a good practice at all.

## [Node.js birth][node-1st-presentation], and the JavaScript revolution

> _"IO has to be done differently, we are doing it wrong. Everything...
  The way we are doing IO makes things difficult."_  
  _- Ryan Dahl_

Node.js took the world of web development by assault.
Being able to write one single language on every end of your web software were a
long time dream of developers - and suddently, it was possible.

Suddently, every

[prototype-www]: http://prototypejs.org/
[scriptaculous-www]: http://script.aculo.us/
[dojo-www]: https://dojotoolkit.org/
[jquery-www]: https://jquery.com/
[node-1st-presentation]: https://www.youtube.com/watch?v=ztspvPYybIY