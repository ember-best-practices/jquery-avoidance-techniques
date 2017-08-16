# Alternatives to `$.data()`


## Option 1:

Use WeakMap instead.

```js
const wMap = new WeakMap();
let pojo = {};

// keys and values can be any objects
wMap.set(pojo, 321);

// 321
wMap.get(pojo);
wMap.get(first);

// true
wMap.has(pojo);

// true
wMap.delete(pojo);
```

---