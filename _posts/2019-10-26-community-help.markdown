---
layout: post
title:  "Let's ask the community"
date:   2019-10-26 12:31:00 +0000
categories: jekyll update
---

Today I've decided to surrender to my inability to attach images to my posts. There is a wonderful place to visit on those situations so I've published the issue on [StackOverflow](https://stackoverflow.com/)

Hopefully there will be a nice wise developer who will loose some time giving me a obvious solution to this =D... And they did!

```
![Image]({{ "/assets/images/old_look.JPG" | absolute_url }})
![Image]({{ "/assets/images/old_look.JPG" | prepend: site.baseurl }})
![Image]("/assets/images/old_look.JPG")
![Image]("../assets/images/old_look.JPG")
```

Those were my options and in the end 2 of them worked! (first and second one).

Nothing more to tell about this for now. See you soon!