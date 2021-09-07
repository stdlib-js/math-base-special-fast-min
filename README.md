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

# min

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] [![dependencies][dependencies-image]][dependencies-url]

> Return the minimum value.

<!-- Section to include introductory text. Make sure to keep an empty line after the intro `section` element and another before the `/section` close. -->

<section class="intro">

</section>

<!-- /.intro -->

<!-- Package usage documentation. -->

<section class="installation">

## Installation

```bash
npm install @stdlib/math-base-special-fast-min
```

</section>

<section class="usage">

## Usage

```javascript
var min = require( '@stdlib/math-base-special-fast-min' );
```

#### min( x, y )

Returns the minimum value.

```javascript
var v = min( 4.2, 3.14 );
// returns 3.14
```

</section>

<!-- /.usage -->

<!-- Package usage notes. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="notes">

## Notes

-   The implementation **ignores** the sign of `0`.

    ```javascript
    var v = min( +0.0, -0.0 );
    // returns -0.0

    v = min( -0.0, +0.0 );
    // returns +0.0
    ```

-   The implementation does **not** check for `NaN` arguments.

    ```javascript
    var v = min( 3.14, NaN );
    // returns NaN

    v = min( NaN, 3.14 );
    // returns 3.14
    ```

</section>

<!-- /.notes -->

<!-- Package usage examples. -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
var minstd = require( '@stdlib/random-base-minstd-shuffle' );
var min = require( '@stdlib/math-base-special-fast-min' );

var x;
var y;
var v;
var i;

for ( i = 0; i < 100; i++ ) {
    x = minstd();
    y = minstd();
    v = min( x, y );
    console.log( 'min(%d,%d) = %d', x, y, v );
}
```

</section>

<!-- /.examples -->

<!-- Section to include cited references. If references are included, add a horizontal rule *before* the section. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="references">

</section>

<!-- /.references -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   [`@stdlib/math/base/special/min`][@stdlib/math/base/special/min]: return the minimum value.

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

Copyright &copy; 2016-2021. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/math-base-special-fast-min.svg
[npm-url]: https://npmjs.org/package/@stdlib/math-base-special-fast-min

[test-image]: https://github.com/stdlib-js/math-base-special-fast-min/actions/workflows/test.yml/badge.svg
[test-url]: https://github.com/stdlib-js/math-base-special-fast-min/actions/workflows/test.yml

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/math-base-special-fast-min/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/math-base-special-fast-min?branch=main

[dependencies-image]: https://img.shields.io/david/stdlib-js/math-base-special-fast-min.svg
[dependencies-url]: https://david-dm.org/stdlib-js/math-base-special-fast-min/main

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/math-base-special-fast-min/main/LICENSE

<!-- <related-links> -->

[@stdlib/math/base/special/min]: https://github.com/stdlib-js/math-base-special-min

<!-- </related-links> -->

</section>

<!-- /.links -->
