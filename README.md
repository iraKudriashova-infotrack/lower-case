# Lower Case

[![NPM version][npm-image]][npm-url]
[![Build status][travis-image]][travis-url]
[![Test coverage][coveralls-image]][coveralls-url]

Lower case a string.

Supports Unicode (non-ASCII characters) and non-string entities, such as objects with a `toString` property, numbers and booleans. Empty values (`null` and `undefined`) will result in an empty string.

## Installation

```sh
npm install lower-case --save
```

## Usage

```js
var lowerCase = require('lower-case');

lowerCase(null);           //=> ""
lowerCase('STRING');       //=> "string"
lowerCase('STRING', 'tr'); //=> "strıng"

upperCase({ toString: function () { return 'TEST'; } }); //=> "test"
```

## License

MIT

[npm-image]: https://img.shields.io/npm/v/lower-case.svg?style=flat
[npm-url]: https://npmjs.org/package/lower-case
[travis-image]: https://img.shields.io/travis/blakeembrey/lower-case.svg?style=flat
[travis-url]: https://travis-ci.org/blakeembrey/lower-case
[coveralls-image]: https://img.shields.io/coveralls/blakeembrey/lower-case.svg?style=flat
[coveralls-url]: https://coveralls.io/r/blakeembrey/lower-case?branch=master
