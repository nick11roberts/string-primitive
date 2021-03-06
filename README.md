String Primitive
===
[![NPM version][npm-image]][npm-url] [![Build Status][travis-image]][travis-url] [![Coverage Status][coveralls-image]][coveralls-url] [![Dependencies][dependencies-image]][dependencies-url]

> Validates if a value is a string primitive.


## Installation

``` bash
$ npm install validate.io-string-primitive
```

For use in the browser, use [browserify](https://github.com/substack/node-browserify).


## Usage

``` javascript
var isString = require( 'validate.io-string-primitive' );
```

#### isString( value )

Validates if a `value` is a `string` primitive.

``` javascript
var value = 'beep';

var bool = isString( value );
// returns true
```


## Examples

``` javascript
var isString = require( 'validate.io-string-primitive' );

console.log( isString( 'beep' ) );
// returns true

console.log( isString( new String( 'beep' ) ) );
// returns false

console.log( isString( 5 ) );
// returns false
```

To run the example code from the top-level application directory,

``` bash
$ node ./examples/index.js
```


## Tests

### Unit

Unit tests use the [Mocha](http://mochajs.org) test framework with [Chai](http://chaijs.com) assertions. To run the tests, execute the following command in the top-level application directory:

``` bash
$ make test
```

All new feature development should have corresponding unit tests to validate correct functionality.


### Test Coverage

This repository uses [Istanbul](https://github.com/gotwarlost/istanbul) as its code coverage tool. To generate a test coverage report, execute the following command in the top-level application directory:

``` bash
$ make test-cov
```

Istanbul creates a `./reports/coverage` directory. To access an HTML version of the report,

``` bash
$ make view-cov
```


---
## License

[MIT license](http://opensource.org/licenses/MIT). 


## Copyright

Copyright &copy; 2015. Athan Reines.


[npm-image]: http://img.shields.io/npm/v/validate.io-string-primitive.svg
[npm-url]: https://npmjs.org/package/validate.io-string-primitive

[travis-image]: http://img.shields.io/travis/validate-io/string-primitive/master.svg
[travis-url]: https://travis-ci.org/validate-io/string-primitive

[coveralls-image]: https://img.shields.io/coveralls/validate-io/string-primitive/master.svg
[coveralls-url]: https://coveralls.io/r/validate-io/string-primitive?branch=master

[dependencies-image]: http://img.shields.io/david/validate-io/string-primitive.svg
[dependencies-url]: https://david-dm.org/validate-io/string-primitive

[dev-dependencies-image]: http://img.shields.io/david/dev/validate-io/string-primitive.svg
[dev-dependencies-url]: https://david-dm.org/dev/validate-io/string-primitive

[github-issues-image]: http://img.shields.io/github/issues/validate-io/string-primitive.svg
[github-issues-url]: https://github.com/validate-io/string-primitive/issues
