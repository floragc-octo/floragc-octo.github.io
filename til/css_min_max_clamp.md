---
layout: layouts/til.njk
title: min(), max(), clamp()
description: 
date: 2022-02-05
tags: ['post', 'css', 'gist']
---

```css
width: 45%;

/* max-width */
max-width: 600px;
width: min(600px, 45%); /* prends la plus petite */

/* min-width */
min-width: 500px;
width: max(500px, 45%); /* prends la plus grande */

/* peut aussi se comparer avec la hauteur */
/* pour prendre la plus petite/grande */
width: min(500px, 45%, 50vh);
width: max(600px, 45%, 50vh);

/* pour combiner */
/* clamp(minimum, ideal, maximum) */
width: clamp(30%, 600px, 80vh)
```