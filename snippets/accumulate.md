---
title: 数组累加
tags: math,array
expertise: intermediate
author: chalarangelo
firstSeen: 2020-05-04T12:20:46+03:00
lastUpdated: 2022-01-30T13:10:13+02:00
---

创建一个数组累加器

- 使用`Array.prototype.reduce()`，初始化为一个空的数组累加器，对`nums`进行迭代。
- 使用`Array.prototype.slice()`来获取前一个累加结果。
- 使用扩展运算符(`...`)将新的总和与之前的总累加到数组中。

```js
const accumulate = (...nums) =>
  nums.reduce((acc, n) => [...acc, n + (acc.slice(-1)[0] || 0)], []);
```

```js
accumulate(1, 2, 3, 4); // [1, 3, 6, 10]
accumulate(...[1, 2, 3, 4]); // [1, 3, 6, 10]
```
