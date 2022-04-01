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

# isEmptyArrayLikeObject

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Test if a value is an empty array-like object.



<section class="usage">

## Usage

```javascript
import isEmptyArrayLikeObject from 'https://cdn.jsdelivr.net/gh/stdlib-js/assert-is-empty-array-like-object@esm/index.mjs';
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
import isEmptyArrayLikeObject from 'https://cdn.jsdelivr.net/gh/stdlib-js/assert-is-empty-array-like-object@esm/index.mjs';

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

Copyright &copy; 2016-2022. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/assert-is-empty-array-like-object.svg
[npm-url]: https://npmjs.org/package/@stdlib/assert-is-empty-array-like-object

[test-image]: https://github.com/stdlib-js/assert-is-empty-array-like-object/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/assert-is-empty-array-like-object/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/assert-is-empty-array-like-object/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/assert-is-empty-array-like-object?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/assert-is-empty-array-like-object.svg
[dependencies-url]: https://david-dm.org/stdlib-js/assert-is-empty-array-like-object/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/assert-is-empty-array-like-object/tree/deno
[umd-url]: https://github.com/stdlib-js/assert-is-empty-array-like-object/tree/umd
[esm-url]: https://github.com/stdlib-js/assert-is-empty-array-like-object/tree/esm

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/assert-is-empty-array-like-object/main/LICENSE

[array-like]: http://www.2ality.com/2013/05/quirk-array-like-objects.html

<!-- <related-links> -->

<!-- </related-links> -->

</section>

<!-- /.links -->