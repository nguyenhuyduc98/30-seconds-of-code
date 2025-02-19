---
title: Product of numeric values
type: snippet
tags: [math]
cover: travel-mug-1
dateModified: 2020-10-22T20:24:04+03:00
---

Calculates the product of two or more numbers/arrays.

- Use `Array.prototype.reduce()` to multiply each value with an accumulator, initialized with a value of `1`.

```js
const prod = (...arr) => [...arr].reduce((acc, val) => acc * val, 1);
```

```js
prod(1, 2, 3, 4); // 24
prod(...[1, 2, 3, 4]); // 24
```
