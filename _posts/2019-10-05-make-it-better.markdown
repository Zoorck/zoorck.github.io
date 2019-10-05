---
layout: post
title:  "Let's make it look better now"
date:   2019-10-05 02:31:00 +0000
categories: jekyll update
---

First of all I just installed jekyll to be able to serve the web in localhost:4000 but it looks like it won't work with the current website file content, so I'll try to build it from scratch since I think I will be able to reuse the posts (which are almost everything I built).

After installing jekyll locally I thought of building my development environment in a docker container but then I felt that it would take to much time before I could actually put some stuff online so maybe I'll be trying this latter on.

Wait! I just installed [Sublime Merge][sublime-merge] to my text editor and it actually worked for the 10th commit of my current website... amazing.

After selecting [cayman][cayman] as my web theme, I'll try to open a branch, create the blog following cayman instructions and we'll see what we can then recycle from the current blog. (and how we marge with the master branch)

I think I created a branch called newlook and after that I started a project with default jekyll commands: jekyll new blog

After that I just coppied all the files to the old folder to be able to run the website in localhost. And it Worked! (almost) I deleted a file and there is a post not being displayed. I'll try to push it to the GitHub repo. Done!

Now I'm gonna try to attach an image denmostrating it, first, let's include this asset in assets/img.

Now the config file: COPY&PASTE time

```
defaults:
  - scope:
      path: "assets/img"
    values:
      image: true
```

Aaaaaaand...

{{ neewlook_branch.png }}

Well, Now i've tryied to insert and image but I'm not being able to show it on localhost, maybe it's because I've been working on newlook branch and not in master branch. I'll marge it and see what happens.

[cayman]: https://github.com/pages-themes/cayman
[sublime-merge]: https://www.sublimemerge.com/