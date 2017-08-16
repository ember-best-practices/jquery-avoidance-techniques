# Alternatives to `$.clone()`


## Option 1:

Use cloneNode instead. !Warning this method may lead to duplicate element IDs in the DOM.

```js
// clone the node WITHOUT child nodes
const clonedNode = el.cloneNode(false);
```

```js
// clone the node WITH child nodes
const clonedNode = el.cloneNode(true);
```

---
