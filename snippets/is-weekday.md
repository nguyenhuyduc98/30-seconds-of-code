---
title: Date is weekday
type: snippet
tags: [date]
cover: typewriter
dateModified: 2020-10-20T23:02:01+03:00
---

Checks if the given date is a weekday.

- Use `Date.prototype.getDay()` to check weekday by using a modulo operator (`%`).
- Omit the argument, `d`, to use the current date as default.

```js
const isWeekday = (d = new Date()) => d.getDay() % 6 !== 0;
```

```js
isWeekday(); // true (if current date is 2019-07-19)
```
