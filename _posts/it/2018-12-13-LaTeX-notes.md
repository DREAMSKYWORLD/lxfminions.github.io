---
layout: post
title: LaTeX notes
categories: [it]
tags: [LaTeX]
date: 2018-12-13
---

{% include toc.html %}

## Beamer
- Beamer themes in [Beamer Theme Matrix](https://hartwork.org/beamer-theme-matrix/)
   ```latex
    \usetheme{Berkeley}
    \usecolortheme{beaver}
   ```

## Tikz
- `+` and `++` operation
  {% highlight latex %}
    \draw (x1, y1) -- +(x2, y2) -- +(x3, y3); % from (x1, y1) to (x1+x2, y1+y2) to (x1+x3, y1+y3)
      \draw (x1, y1) -- +(x2, y2) -- ++(x3, y3); % from (x1, y1) to (x1+x2, y1+y2) to (x1+x2+x3, y1+y2+y3)
  {% endhighlight %}
