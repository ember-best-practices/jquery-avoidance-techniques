# Alternatives to `$.css()`


## Option 1:

Use getComputedStyle instead. !Please note `getComputedStyle` triggers a reflow/recalc.

```js
// get entire CSSStyleDeclaration Object
getComputedStyle(elem);
```

```js
// get a specific style (in this example 'color')
getComputedStyle(elem)['color'];
```

---


## Option 2:

Use elem#style instead.

```js
elem.style.borderWidth = '20px';
```

---
