---
title: "TIL: Multiple Backgrounds with CSS background"
layout: post
date: 30 Jun 2021 20:28
headerImage: false
tag:
- background-images
- til
- css
category: blog
author: ritikpatni
description: Learned about using multiple background images in a single tag with CSS
---

Today I discovered a clever trick with CSS background images. It's possible with CSS to have multiple images in a single background-image tag, which is unique and can come in handy for many use cases.

## How to do it

```html
<section>
<section />
```

```css
section {
  background-image: url("https://source.unsplash.com/random/150x150"),
    url("https://source.unsplash.com/random/150x200"),
    url("https://source.unsplash.com/random/150x250"),
    linear-gradient(
      90deg,
      rgba(52, 130, 253, 1) 43%,
      rgba(255, 255, 255, 1) 80%
    );
  background-position: top left, bottom right, center;
  background-repeat: no-repeat;
  height: 300px;
  width: 100%;
}
```

### You can also play with this here

<p class="codepen" data-height="300" data-default-tab="html,result" data-slug-hash="eYWNxqr" data-editable="true" data-user="ritikpatni" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/ritikpatni/pen/eYWNxqr">
  Multiple Background Images</a> by Ritik Patni (<a href="https://codepen.io/ritikpatni">@ritikpatni</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

