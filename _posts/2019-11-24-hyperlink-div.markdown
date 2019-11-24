---
layout: post
title:  "Hyperlinking div"
date:   2019-11-24 00:00:00 +0000
categories: jekyll update
---

After remaking the banner text I've decided to link the three div sections after the banner, I found this example:

```
<div onclick="location.href='newurl.html';"> content </div>
```

And I made this adaption to fulfill my interests:

```
<div class="flex-child" onclick="location.href='{{ "/posts/" | prepend: site.baseurl }}';">
```
Once the other sections star, I'll be able to link them too. Now I'm going to try to change the cursor when hovering on top of the divs. I think it's as easy as:

```
.flex-child {
	cursor: pointer;
}
```