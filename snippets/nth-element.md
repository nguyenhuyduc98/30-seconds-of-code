---
title: Nth element
type: snippet
tags: [array]
cover: laptop-plants
dateModified: 2020-10-21T21:54:53+03:00
---

Returns the nth element of an array.

- Use `Array.prototype.slice()` to get an array containing the nth element at the first place.
- If the index is out of bounds, return `undefined`.
- Omit the second argument, `n`, to get the first element of the array.

```js
const nthElement = (arr, n = 0) =>
  (n === -1 ? arr.slice(n) : arr.slice(n, n + 1))[0];
```

```js
nthElement(['a', 'b', 'c'], 1); // 'b'
nthElement(['a', 'b', 'b'], -3); // 'a'
```
