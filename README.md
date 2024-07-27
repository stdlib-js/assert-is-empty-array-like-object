<!--

@license Apache-2.0

Copyright (c) 2021 The Stdlib Authors.

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

# isEmptyArrayLikeObject

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Test if a value is an empty array-like object.



<section class="usage">

## Usage

```javascript
import isEmptyArrayLikeObject from 'https://cdn.jsdelivr.net/gh/stdlib-js/assert-is-empty-array-like-object@v0.2.2-esm/index.mjs';
```

#### isEmptyArrayLikeObject( value )

Tests if a value is an empty [array-like][array-like] `object`.

<!-- eslint-disable object-curly-newline -->

```javascript
var bool = isEmptyArrayLikeObject( [] );
// returns true

bool = isEmptyArrayLikeObject( { 'length': 0 } );
// returns true
```

If provided a `string`, the function returns `false`.

```javascript
var bool = isEmptyArrayLikeObject( '' );
// returns false
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint-disable object-curly-newline, object-curly-spacing, no-empty-function, no-restricted-syntax -->

<!-- eslint no-undef: "error" -->

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="module">

import Float64Array from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-float64@esm/index.mjs';
import isEmptyArrayLikeObject from 'https://cdn.jsdelivr.net/gh/stdlib-js/assert-is-empty-array-like-object@v0.2.2-esm/index.mjs';

var bool = isEmptyArrayLikeObject( { 'length': 0 } );
// returns true

bool = isEmptyArrayLikeObject( [] );
// returns true

bool = isEmptyArrayLikeObject( new Float64Array( [] ) );
// returns true

bool = isEmptyArrayLikeObject( 'beep' );
// returns false

bool = isEmptyArrayLikeObject( null );
// returns false

bool = isEmptyArrayLikeObject( void 0 );
// returns false

bool = isEmptyArrayLikeObject( 5 );
// returns false

bool = isEmptyArrayLikeObject( true );
// returns false

bool = isEmptyArrayLikeObject( {} );
// returns false

bool = isEmptyArrayLikeObject( function noop() {} );
// returns false

</script>
</body>
</html>
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/assert-is-array-like-object`][@stdlib/assert/is-array-like-object]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object.</span>
-   <span class="package-name">[`@stdlib/assert-is-empty-array`][@stdlib/assert/is-empty-array]</span><span class="delimiter">: </span><span class="description">test if a value is an empty array.</span>
-   <span class="package-name">[`@stdlib/assert-is-empty-collection`][@stdlib/assert/is-empty-collection]</span><span class="delimiter">: </span><span class="description">test if a value is an empty collection.</span>

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

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

[npm-image]: http://img.shields.io/npm/v/@stdlib/assert-is-empty-array-like-object.svg
[npm-url]: https://npmjs.org/package/@stdlib/assert-is-empty-array-like-object

[test-image]: https://github.com/stdlib-js/assert-is-empty-array-like-object/actions/workflows/test.yml/badge.svg?branch=v0.2.2
[test-url]: https://github.com/stdlib-js/assert-is-empty-array-like-object/actions/workflows/test.yml?query=branch:v0.2.2

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/assert-is-empty-array-like-object/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/assert-is-empty-array-like-object?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/assert-is-empty-array-like-object.svg
[dependencies-url]: https://david-dm.org/stdlib-js/assert-is-empty-array-like-object/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/assert-is-empty-array-like-object/tree/deno
[deno-readme]: https://github.com/stdlib-js/assert-is-empty-array-like-object/blob/deno/README.md
[umd-url]: https://github.com/stdlib-js/assert-is-empty-array-like-object/tree/umd
[umd-readme]: https://github.com/stdlib-js/assert-is-empty-array-like-object/blob/umd/README.md
[esm-url]: https://github.com/stdlib-js/assert-is-empty-array-like-object/tree/esm
[esm-readme]: https://github.com/stdlib-js/assert-is-empty-array-like-object/blob/esm/README.md
[branches-url]: https://github.com/stdlib-js/assert-is-empty-array-like-object/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/assert-is-empty-array-like-object/main/LICENSE

[array-like]: http://www.2ality.com/2013/05/quirk-array-like-objects.html

<!-- <related-links> -->

[@stdlib/assert/is-array-like-object]: https://github.com/stdlib-js/assert-is-array-like-object/tree/esm

[@stdlib/assert/is-empty-array]: https://github.com/stdlib-js/assert-is-empty-array/tree/esm

[@stdlib/assert/is-empty-collection]: https://github.com/stdlib-js/assert-is-empty-collection/tree/esm

<!-- </related-links> -->

</section>

<!-- /.links -->
