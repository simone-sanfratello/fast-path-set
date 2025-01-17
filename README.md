# fast-path-set

A fast drop-in replacement for [`lodash.set`](https://www.npmjs.com/package/lodash.set).

## Install 

```
$ npm i fast-path-set --save
```

## Usage

```js
const set = require('fast-path-set')
const obj = {}
set(obj, 'a.b.c', 1)
console.log(obj.a.b.c)
```

## Benchmark

```
$ npm i lodash.set
$ node bench.js lodash.set
89006.61856603622
$ npm i dset
$ node bench.js dset
70376.78514885902
$ node bench.js fast-path-set
34950.48910498619
```

## License

MIT
