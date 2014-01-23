---
layout: post
comments: true
share: true
title: Git Branch From Stash
tag: git
---

I often save unfinished work in a stash and later want to create a new branch from it.  I used to create a branch and apply the stash until I stumbled upon this great shortcut:

    git stash branch \<branchname> [\<stash>]
    
From the docs:

>Creates and checks out a new branch named <branchname> starting from the commit at which the <stash> was originally created, applies the changes recorded in <stash> to the new working tree and index. If that succeeds, and <stash> is a reference of the form stash@{<revision>}, it then drops the <stash>. When no <stash> is given, applies the latest one.
