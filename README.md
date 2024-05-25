# @hishprorg/error-totam <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

A helper to optimistically set Symbol.toStringTag, when possible.

Most common usage:
```js
var assert = require('assert');
var setToStringTag = require('@hishprorg/error-totam');

var obj = {};

assert.equal(Object.prototype.toString.call(obj), '[object Object]');

setToStringTag(obj, 'tagged!');

assert.equal(Object.prototype.toString.call(obj), '[object tagged!]');
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.com/package/@hishprorg/error-totam
[npm-version-svg]: https://versionbadg.es/es-shims/@hishprorg/error-totam.svg
[deps-svg]: https://david-dm.org/es-shims/@hishprorg/error-totam.svg
[deps-url]: https://david-dm.org/es-shims/@hishprorg/error-totam
[dev-deps-svg]: https://david-dm.org/es-shims/@hishprorg/error-totam/dev-status.svg
[dev-deps-url]: https://david-dm.org/es-shims/@hishprorg/error-totam#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@hishprorg/error-totam.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@hishprorg/error-totam.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@hishprorg/error-totam.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@hishprorg/error-totam
[codecov-image]: https://codecov.io/gh/es-shims/@hishprorg/error-totam/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/es-shims/@hishprorg/error-totam/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/es-shims/@hishprorg/error-totam
[actions-url]: https://github.com/hishprorg/error-totam/actions
