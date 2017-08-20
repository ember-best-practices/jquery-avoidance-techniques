# Alternatives to `$.text()`


## Option 1:

Use `textContent` instead.

```html
<div class="elem">My name is <span class="bold">Tomster</span></div>
```

```js
const elem = document.querySelector('.elem');
const text = elem.textContent; // "My name is Tomster"
```


---
