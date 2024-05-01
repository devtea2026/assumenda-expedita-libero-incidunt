# @devtea2026/assumenda-expedita-libero-incidunt <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

Is this value a JS Map? This module works cross-realm/iframe, and despite ES6 @@toStringTag.

## Example

```js
var isMap = require('@devtea2026/assumenda-expedita-libero-incidunt');
assert(!isMap(function () {}));
assert(!isMap(null));
assert(!isMap(function* () { yield 42; return Infinity; });
assert(!isMap(Symbol('foo')));
assert(!isMap(1n));
assert(!isMap(Object(1n)));

assert(!isMap(new Set()));
assert(!isMap(new WeakSet()));
assert(!isMap(new WeakMap()));

assert(isMap(new Map()));

class MyMap extends Map {}
assert(isMap(new MyMap()));
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@devtea2026/assumenda-expedita-libero-incidunt
[npm-version-svg]: https://versionbadg.es/inspect-js/@devtea2026/assumenda-expedita-libero-incidunt.svg
[deps-svg]: https://david-dm.org/inspect-js/@devtea2026/assumenda-expedita-libero-incidunt.svg
[deps-url]: https://david-dm.org/inspect-js/@devtea2026/assumenda-expedita-libero-incidunt
[dev-deps-svg]: https://david-dm.org/inspect-js/@devtea2026/assumenda-expedita-libero-incidunt/dev-status.svg
[dev-deps-url]: https://david-dm.org/inspect-js/@devtea2026/assumenda-expedita-libero-incidunt#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@devtea2026/assumenda-expedita-libero-incidunt.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@devtea2026/assumenda-expedita-libero-incidunt.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@devtea2026/assumenda-expedita-libero-incidunt.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@devtea2026/assumenda-expedita-libero-incidunt
[codecov-image]: https://codecov.io/gh/inspect-js/@devtea2026/assumenda-expedita-libero-incidunt/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@devtea2026/assumenda-expedita-libero-incidunt/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@devtea2026/assumenda-expedita-libero-incidunt
[actions-url]: https://github.com/devtea2026/assumenda-expedita-libero-incidunt/actions
