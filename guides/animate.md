# Alternatives to `$.animate()`


## Option 1:

Use CSS animations instead toggled with JS classList#add and classList#remove.

```js
el.classList.add('show');
el.classList.remove('hide');
```

```css
.show {
  transition: opacity 200ms;
}
.hide {
  opacity: 0;
}
```

---