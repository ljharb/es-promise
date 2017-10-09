## Promise

A promise implementation of Promises/A+, and with es7 promise enhancements.

Author: Allex Wang (allex.wxn@gmail.com)

*Note:*

- Support `Promise.try()`, `#.finally()`
- Provide `Promise.polyfill()` api and entry `dist/promise.polyfill.min.js`

## Installation

NPM

```sh
npm i @fedor/promise
```

Combo

```html
<script src="//s1.analysys.cn/libs/??-/@fedor/promise@1.0.0/dist/promise.polyfill.min.js"></script>
```

### Auto-polyfill

To polyfill the global environment (either in Node or in the browser via CommonJS) use the following code snippet:

```js
require('@fedor/promise').polyfill();
```

Alternatively

```js
require('@fedor/promise/dist/promise.polyfill');
```

Notice that we don't assign the result of `polyfill()` to any variable. The `polyfill()` method will patch the global
environment (in this case to the Promise name) when called.


## License

MIT
