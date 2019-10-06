---
layout: post
title:  "Start with a guide for beginers"
date:   2019-10-05 14:31:00 +0000
categories: jekyll update
---

After reading [Creating and Hosting a Personal Site on GitHub][cayman] i just understood some more about jeckyll but the truth is I'm still not sure on how URLs work in jekyll + GitHub pages and why my assets are not properly displayed in my blog, so let's try on some more research.

![A beautyfull cat](https://upload.wikimedia.org/wikipedia/commons/3/38/Adorable-animal-cat-20787.jpg) 

I found this image and it looks like we can store images over the internet but not in the local Repo... well, it's not what I wanted to do but it's a start.

At least, I'm not so frustrated now. Easy guide following [this video](https://www.youtube.com/watch?v=afFb_DcBBdA)

Why it's now working in the GitHub Pages repo now? Date and time issues, I'm not sure to have the right configuration both in my local system and GitHub atomated datetime.

I may want to find a way to fix this adding a +1h to all posts. Yes, that's it, I'm in Spain so... Not sure if this is a real fix for the problem.

I just found [this post](https://mehmandarov.com/jekyll-content-on-time/) where a good explanation on how to establish Jekyll date and time zone and this [other wiki post](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones) where all the time zone options are displayed.

```
# set timezone
timezone: Europe/Madrid
```

I just started to find warnings when adding changes to staging with git. (I'm starting to feel like a pro with git even though I only use 3 commends) It's related to some sort of file that Jekyll is authomatically generating in the cache folder. I really don't know why this folder is there but it keeps changing a lot on every commit.

Well the warning is about a LF being changed to CRLF and the original line endings in my working directory... let's google.

I just found it is related to the way Unix systems treat line endings, or **Line feeds = LF**. I'll just copy paste and [reference](https://stackoverflow.com/questions/5834014/lf-will-be-replaced-by-crlf-in-git-what-is-that-and-is-it-important) to the original onswer:

_In Unix systems the end of a line is represented with a line feed (LF). In windows a line is represented with a carriage return (CR) and a line feed (LF) thus (CRLF). when you get code from git that was uploaded from a unix system they will only have an LF._

_If you want to turn this warning off, type this in the git command line:_
```
git config core.autocrlf true
```
_If you want to make an intelligent decision how git should handle this, read [the documentation](https://git-scm.com/book/en/v2/Customizing-Git-Git-Configuration#Formatting-and-Whitespace)_



[cayman]: https://github.com/pages-themes/cayman

