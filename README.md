# Consentua Blog

[blog.consentua.com](http://blog.consentua.com)

> Jekyll blog for [Consentua](http://Consentua.com) hosted on github pages. Forked from [Hyde](https://github.com/poole/hyde)

## How do I 'do' a blog post??

In github or in [prose.io](http://prose.io/) login with an account able to edit this repo; go to `_posts` there you can see other posts including the example post.

Have a look inside the example post, use this file as a guide on how to write a blog post.

Posts require a few things to work:
* correct file name structure eg `2012-02-07-example-content.md` with date with dashes, and post title.
* have the following configurations at the top of the file:

example config
```
---
layout: post
title: Example content
published: true
author: jack_mason
comments: true
---

# Content ...
```

* `layout: post` - is required to function as a post
* `title:` - title of the post (be the same as in the file name)
* `published:` - can be ture or false, if false the post wont display on the blog; this means you can work on a blog post without it bieng visible to anyone.
* `author:` - the author of the post, see `_data/authors.yml` to see valid author details.
* `comments:` - enables / disables the comments at the bottom of the blog post.


## How do I run on my local machine?

Clone or fork this repo,
make sure you have ruby and jekyll installed on your machine, and run:

install dependencies:
` gem install -g `

and serve: 
```
$ jekyll serve
# => A development server will run at http://localhost:4000/
# Auto-regeneration: enabled. Use `--no-watch` to disable.
```

## How do I deploy?

To deploy to github pages, just commit and push your changes to github.
