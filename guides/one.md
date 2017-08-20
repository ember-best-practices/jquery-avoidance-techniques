# Alternatives to `$.one()`


## Option 1:

Use elem#addEventListener with the `once` option instead.
*NOTE:* This is not currently supported in Edge/Internet Explorer ([support](http://caniuse.com/#search=once))

```js
document.querySelector('.elem').addEventListener('click', clickHandler, { once: true });
```

---


## Option 2:

Create an event listener that cancels itself manually.

```js
const elem = document.querySelector('.elem');

const clickHandler = () => {
    console.log('I have been clicked only once');
    elem.removeEventListener('click', clickHandler);
};

elem.addEventListener('click', clickHandler);
```

---
