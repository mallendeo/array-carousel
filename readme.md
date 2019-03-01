# array-carousel

Navigate through an array indefinitely. This allows you to use negative and out of range indexes on any given array.

## Install

```bash
$ yarn add array-carousel # or npm i array-carousel
```

## Usage

```js
const carousel = require('array-carousel');

// Adds infinite (positive and negative) index support to any given array
const unicorn = carousel(['pony', 'cake', 'rainbow']);

console.log(unicorn[-1]) // 'rainbow'
console.log(unicorn[-9]) //'pony'
console.log(unicorn[4]) // 'cake'

unicorn[1] = null
console.log(unicorn[1]) // null
```

## License

MIT
