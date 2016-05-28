# json-property-filter

[![MIT License][license-image]][license-url] [![npm version][npmjs-image]][npmjs-url] [![Build Status][travis-image]][travis-url] [![typescript-standard-style][standard-image]][standard-url] [![david-dm Status][david-image]][david-url] [![david-dm devDependency Status][david-dev-dependencies-image]][david-dev-dependencies-url]

A library to filter a JSON object by including/excluding properties.

## Installation

```bash
$ npm install json-property-filter
```

## Usage

To using [TypeScript](https://www.typescriptlang.org/) or JavaScript (ES6 support) language:

```javascript
import {JsonPropertyFilter} from "json-property-filter";

var filter = new JsonPropertyFilter(["**"]);
filter.apply({ key: "value" });
```

If you use JavaScript (ES5 support) language:

```javascript
var JsonPropertyFilter = require("json-property-filter");

var filter = new JsonPropertyFilter.JsonPropertyFilter(["**"]);
filter.apply({ key: "value" });
```

### Filters

- `**`

All properties. Include all the properties children and their children.

- `*`

Root properties only. Include only properties located in the root.

- `root.property.element`

Specific property. Include a specific property.

### TypeScript definition

If you use the TypeScript language on your project, you can use the following definition from that path:

> lib/jsonPropertyFilter.d.ts

### Test

```bash
$ npm install -g typings
$ npm install
$ typings install

$ npm test
```

## License

> The MIT License (MIT)

> Copyright (c) 2016 Cyril Schumacher.fr

> Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

> The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

[david-dev-dependencies-image]: https://david-dm.org/cyrilschumacher/json-property-filter/dev-status.svg
[david-dev-dependencies-url]: https://david-dm.org/cyrilschumacher/json-property-filter#info=devDependencies
[david-image]: https://david-dm.org/cyrilschumacher/json-property-filter.svg
[david-url]: https://david-dm.org/cyrilschumacher/json-property-filter
[license-image]: http://img.shields.io/badge/license-MIT-blue.svg?style=flat
[license-url]: LICENSE
[npmjs-image]: https://badge.fury.io/js/json-property-filter.svg
[npmjs-url]: https://www.npmjs.com/package/json-property-filter
[standard-image]: https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat
[standard-url]: https://github.com/Microsoft/TypeScript/wiki/Coding-guidelines
[travis-image]: https://travis-ci.org/cyrilschumacher/json-property-filter.svg
[travis-url]: https://travis-ci.org/cyrilschumacher/json-property-filter
