---
layout: post
title:  "New web developments in django"
date:   2020-03-06 00:00:00 +0000
categories: jekyll update
---

It looks like it was yesterday I just started this blog and now I've started a new project based in Django! You can check it at zoorck.pythonanywhere.com with an account... which really doesn't look like something useful fr you now.

```
<div onclick="location.href='newurl.html';"> content </div>
```

And I made this adaption to fulfill my interests:

```
<div class="flex-child" onclick="location.href='{{ "/posts/" | prepend: site.baseurl }}';">
```
Once the other sections start, I'll be able to link them too. Now I'm going to try to change the cursor when hovering on top of the divs. I think it's as easy as:

```
.flex-child {
	cursor: pointer;
}
```

Yes it is!