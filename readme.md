# [joelwallis.github.io](http://joelwallis.github.io)

My personal blog.

I try my best to keep some quality on published content, thus
maximizing its usefulness. If you find a bug, mistake or a typo, please
[open an issue][issues:new].

## Participate

I use the GitHub issue tracker to manage the publishing workflow.
Use it to participate, upvoting an article you would like to have me writing
about, or even suggesting a new one.

- [List of pending articles][issues:pending-articles]
- [Request a new article][issues:new]

## Contribute

If you would like to contribute, or you're forking it to make your own blog
(yep, you can do it!), here are the instructions you need to follow in order to
run it locally.

_It uses [Jekyll][jekyll:site], which depends on [Ruby][ruby:site],
[RubyGems][rubygems:site] and [Bundler][bundler:site], so you must have them
installed on your system.
Please refer to their website for installation instructions._

**Clone the repo and install dependencies**

```
$ git clone https://github.com/joelwallis/joelwallis.github.io.git
$ cd joelwallis.github.io
$ bundle install
```

**Start the development server**

```
$ bundle exec jekyll serve
```

[bundler:site]: http://bundler.io
[issues:pending-articles]: https://github.com/joelwallis/joelwallis.github.io/issues?q=is%3Aopen+is%3Aissue+label%3Aarticle
[issues:new]: https://github.com/joelwallis/joelwallis.github.io/issues/new
[jekyll:site]: http://jekyllrb.com
[ruby:site]: https://www.ruby-lang.org
[rubygems:site]: https://rubygems.org
