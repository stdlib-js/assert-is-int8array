<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

# isInt8Array

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Test if a value is an [Int8Array][mdn-int8array].

<section class="installation">

## Installation

```bash
npm install @stdlib/assert-is-int8array
```

Alternatively,

-   To load the package in a website via a `script` tag without installation and bundlers, use the [ES Module][es-module] available on the [`esm` branch][esm-url].
-   If you are using Deno, visit the [`deno` branch][deno-url].
-   For use in Observable, or in browser/node environments, use the [Universal Module Definition (UMD)][umd] build available on the [`umd` branch][umd-url].

The [branches.md][branches-url] file summarizes the available branches and displays a diagram illustrating their relationships.

</section>

<section class="usage">

## Usage

```javascript
var isInt8Array = require( '@stdlib/assert-is-int8array' );
```

#### isInt8Array( value )

Tests if a value is an [`Int8Array`][mdn-int8array].

```javascript
var Int8Array = require( '@stdlib/array-int8' );

var bool = isInt8Array( new Int8Array( 10 ) );
// returns true

bool = isInt8Array( [] );
// returns false
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
var Int8Array = require( '@stdlib/array-int8' );
var Uint8Array = require( '@stdlib/array-uint8' );
var Uint8ClampedArray = require( '@stdlib/array-uint8c' );
var Int16Array = require( '@stdlib/array-int16' );
var Uint16Array = require( '@stdlib/array-uint16' );
var Int32Array = require( '@stdlib/array-int32' );
var Uint32Array = require( '@stdlib/array-uint32' );
var Float32Array = require( '@stdlib/array-float32' );
var Float64Array = require( '@stdlib/array-float64' );
var isInt8Array = require( '@stdlib/assert-is-int8array' );

var bool = isInt8Array( new Int8Array( 10 ) );
// returns true

bool = isInt8Array( new Uint8Array( 10 ) );
// returns false

bool = isInt8Array( new Uint8ClampedArray( 10 ) );
// returns false

bool = isInt8Array( new Int16Array( 10 ) );
// returns false

bool = isInt8Array( new Uint16Array( 10 ) );
// returns false

bool = isInt8Array( new Int32Array( 10 ) );
// returns false

bool = isInt8Array( new Uint32Array( 10 ) );
// returns false

bool = isInt8Array( new Float32Array( 10 ) );
// returns false

bool = isInt8Array( new Float64Array( 10 ) );
// returns false

bool = isInt8Array( new Array( 10 ) );
// returns false

bool = isInt8Array( {} );
// returns false

bool = isInt8Array( null );
// returns false
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/assert-is-int16array`][@stdlib/assert/is-int16array]</span><span class="delimiter">: </span><span class="description">test if a value is an Int16Array.</span>
-   <span class="package-name">[`@stdlib/assert-is-int32array`][@stdlib/assert/is-int32array]</span><span class="delimiter">: </span><span class="description">test if a value is an Int32Array.</span>

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2024. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/assert-is-int8array.svg
[npm-url]: https://npmjs.org/package/@stdlib/assert-is-int8array

[test-image]: https://github.com/stdlib-js/assert-is-int8array/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/assert-is-int8array/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/assert-is-int8array/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/assert-is-int8array?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/assert-is-int8array.svg
[dependencies-url]: https://david-dm.org/stdlib-js/assert-is-int8array/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/assert-is-int8array/tree/deno
[umd-url]: https://github.com/stdlib-js/assert-is-int8array/tree/umd
[esm-url]: https://github.com/stdlib-js/assert-is-int8array/tree/esm
[branches-url]: https://github.com/stdlib-js/assert-is-int8array/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/assert-is-int8array/main/LICENSE

[mdn-int8array]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Int8Array

<!-- <related-links> -->

[@stdlib/assert/is-int16array]: https://github.com/stdlib-js/assert-is-int16array

[@stdlib/assert/is-int32array]: https://github.com/stdlib-js/assert-is-int32array

<!-- </related-links> -->

</section>

<!-- /.links -->
