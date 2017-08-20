# Alternatives to `$.css()`


## Option 1:

Use elem#style instead.

```js
// Getting a style
elem.style.color; // "blue"

// Setting a style
elem.style.borderWidth = '20px';
```

---


## Option 2:

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
