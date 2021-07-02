---
title: "Learned about debugging in Obsidian and adding custom CSS"
layout: post
date: 03 Jun 2021 09:05
headerImage: false
tag:
- obsidian
- til
- css
category: blog
author: ritikpatni
description: Learned a new thing
---

Today when I was checking out preview mode for one of my notes I noticed that emojis were taking complete line instead of staying in the same line which annoyed me because it was looking really weird. After a bit of googling I figured out that it was because the emojis in Obsidian are rendered as `<image>` tags as it was currently taking `display: block`.

## Fix for the problem

```css
.emoji{
    display: inline-block
}
```

Adding the above snippet solves the problem as it makes the display `inline-block` which doesn't use separate line.
