---
layout: post
comments: true
share: true
title: Git - How To Bypass Staging Area
tag: git
---

When I'm working on a quick fix, it can be an annoyance to `git add` the file I was just working on. I just recently learned a little trick to bypass the staging area altogether.

You can run `git commit -a` to automatically add your working copy changes to the staging area and commit them. Note that this will only add changes from tracked files.
