---
published: false
layout: post
title:  "Authenticable models in Ruby on Rails"
permalink: rails-authenticable-models.html
tags: ruby, ruby on rails
---

Today I stumbled upon `ActiveModel::SecurePassword` module while working on a
Ruby on Rails app. It was so easy to turn a model into a password authenticable
entity that I decided to write about.

It works directly in your model. You just need to add a call to
`has_secure_password` on your model class and the magic will happen:

```rb
class User < ApplicationRecord
  has_secure_password
end
```

This function will add two virtual attributes
