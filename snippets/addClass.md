---
title: 给元素添加 class 属性
tags: browser
expertise: beginner
author: chalarangelo
cover: blog_images/budapest-palace.jpg
firstSeen: 2020-12-30T19:21:15+02:00
lastUpdated: 2020-12-30T19:21:15+02:00
---

向HTML元素添加一个class属性。

- 使用`Element.classList`将指定的class属性添加到元素中。

```js
const addClass = (el, className) => el.classList.add(className);
```

```js
addClass(document.querySelector('p'), 'special');
// The paragraph will now have the 'special' class
```
