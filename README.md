# Document Ready

Wait until document is ready.

[This code](https://gist.github.com/tjbenton/4186f003329c623e53f5d4a31744b054) "monkey patched" a ready function onto `document`, I adopted it to not do the monkey patch.

### Usage

```js
import isReady from 'document-ready'

isReady().then(() => {
    // document ready, do stuff
})
```

or using async

```js
let do = async () => {
    await isReady()
    // do stuff
}
```