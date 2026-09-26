+++
title = 'Case insensitive filesystems'
date = 2026-09-26
draft = false
tags = ['dev', 'rant']
description = "Filesystem quirk"
+++

I want to be clear here, why would a file system be case insensitive? Imagine this: you use Windows®, MacOS, or whatever, you have a file named `hello.txt` and you try to create another one with the name `Hello.txt`. Guess what? THOSE ARE IDENTICAL. Well I get the idea that some people don't care enough of the filename case. But as a developer this is counter intuitive. I'm glad I move to a "developer friendly" environment such as Linux[^1], whereas its filesystem, name; btrfs, ext4, etc are case sensitive by default.

## why do I care?
One time me and my friends were on a project. I reviewed my friend's code and it LGTM, because it clearly works on their machine (my mistake for believing this), I tried it on my machine wonders why isn't something working? Why is it complaining of a missing file? As it turns out my friend OS (Windows) is case insensitive and mine (Linux) is case sensitive, my system cant find a specific file because it's every so slightly different. If you're curious me and my friends were making a website.

Why not blame my system? Well my eyes don't decieve. It is in theory: **DIFFERENT**.

## but wait there is an advantages!
I get it, it avoids confusion like: why is my `hello.txt` empty? Ah, as it turns out I put all of my useless notes in `heLlo.txt` silly me! Honestly this has happened to me, in terms of frequency it's probably ≤2 times. Maybe thats because I pay too much attention to details or something? Or it's just so I'm just so used to stare at my computer for whole life?

## Footnote
[^1]: Specifically GNU/Linux or GNU+Linux
