# Alternatives to `$.deferred()`


## Option 1:

Use Promise instead.

```js
const somePromise = new Promise((resolve, reject) => {
  // do something that will call either resolve() or reject()
  // resolve(someVal);
  // OR
  // reject('failed because of some reason...')
});


somePromise.then((success) => {
  // if this was called then the promise was resolvd successfully 
});
```

---