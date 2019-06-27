# Asserting spy call order in sinon

```js
const spy1 = sinon.spy();
const spy2 = sinon.spy();

// invoke your code

sinon.assert.callOrder(spy1, spy2, ...)
```
