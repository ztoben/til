# Custom Blur Handlers

Easily check if you focusing on an element outside of a desired node tree.

```js
onBlur = (e) => {
  if ( !e.currentTarget.contains( e.relatedTarget ) ) {
    console.log('blur event');
  }
}

render() {
  return (
    <div onBlur={this.onBlur}>
      ..
    </div>
  )
}
```

Found [here](https://stackoverflow.com/a/54956308/4202761).
