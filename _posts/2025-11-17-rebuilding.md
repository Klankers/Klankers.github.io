---
layout: post
title: "Rebuilding the website"
date: 2025-11-17
categories: blog
  - blog
  - programming
---
Huzzah! It has returned!

This post will probably have no obvious time discrepancy from the others, but believe it or not, it marks the first post in about a year. It was mostly laziness, combined with a desire not to put too much miscellany on a new machine. I wrote up a series of posts in markdown in `Obsidian` of all places but never cloned my website repo to actually push them because, well, setting up Jekyll locally on Windows and MacOS was something that I knew could take me a whole afternoon.

*Until now.*

I'm in a good situation where I'm currently surrounded by Linux users. We've got an Ubuntu guy and a KDE developer. We all specialize in Python, but that's not the main concern. The fact that I'll be routinely working in Linux means that I might as well reinstall the site and see if I can get it back up and running. It's good practice and I've got folks around me that understand the syntax that's advanced since Ubuntu... 12.04? It's been a while, okay?

And oh my gosh, it's so easy on Linux.

The [Linux instructions](https://jekyllrb.com/docs/installation/ubuntu/) for Jekyll are remarkably short. Install Ruby without needing some big installer image. Get all the prereqs with it while you're at it. Four lines of code for best-practice purposes and wrap it all up by installing the Jekyll bundler. Then I just cloned the old repo, deleted my `Gemfile.lock` (as several of them had depreciated and the bundler would be underpinned to something old), rebuilt it using `bundle install` and then just ran the old `bundle exec jekyll serve`. Easy peasy. No pulling my hair out about figuring out the version of Ruby that comes with MacOS. Don't need Chruby.

<blockquote style="text-align: center;">
  "It just works." - Todd Howard
</blockquote>
