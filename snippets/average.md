---
title: Average of numbers
type: snippet
tags: [math]
cover: interior-8
dateModified: 2020-10-22T20:23:47+03:00
---

Calculates the average of two or more numbers.

- Use `Array.prototype.reduce()` to add each value to an accumulator, initialized with a value of `0`.
- Divide the resulting array by its length.

```js
const average = (...nums) =>
  nums.reduce((acc, val) => acc + val, 0) / nums.length;
```

```js
average(...[1, 2, 3]); // 2
average(1, 2, 3); // 2
```
