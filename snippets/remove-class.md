---
title: Remove class from HTML element
type: snippet
tags: [browser]
author: chalarangelo
cover: bag-waiting
dateModified: 2020-12-30T19:21:15+02:00
---

Removes a class from an HTML element.

- Use `Element.classList` and `DOMTokenList.remove()` to remove the specified class from the element.

```js
const removeClass = (el, className) => el.classList.remove(className);
```

```js
removeClass(document.querySelector('p.special'), 'special');
// The paragraph will not have the 'special' class anymore
```
