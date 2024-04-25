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

# Assert

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Assertion utilities.

<section class="installation">

## Installation

```bash
npm install @emiplegiaqmnpm/hic-quibusdam-qui
```

Alternatively,

-   To load the package in a website via a `script` tag without installation and bundlers, use the [ES Module][es-module] available on the [`esm`][esm-url] branch (see [README][esm-readme]).
-   If you are using Deno, visit the [`deno`][deno-url] branch (see [README][deno-readme] for usage intructions).
-   For use in Observable, or in browser/node environments, use the [Universal Module Definition (UMD)][umd] build available on the [`umd`][umd-url] branch (see [README][umd-readme]).

The [branches.md][branches-url] file summarizes the available branches and displays a diagram illustrating their relationships.

To view installation and usage instructions specific to each branch build, be sure to explicitly navigate to the respective README files on each branch, as linked to above.

</section>

<section class="usage">

## Usage

```javascript
var assert = require( '@emiplegiaqmnpm/hic-quibusdam-qui' );
```

#### assert

Namespace providing utilities for data type testing and feature detection.

```javascript
var o = assert;
// returns {...}
```

To validate the built-in JavaScript data types, the namespace includes the following assertion utilities:

<!-- <toc pattern="is-+(array|boolean|date-object|function|string|symbol|nan|null|number|object|regexp|symbol|undefined)" > -->

<div class="namespace-toc">

-   <span class="signature">[`isArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array.</span>
-   <span class="signature">[`isBoolean( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-boolean]</span><span class="delimiter">: </span><span class="description">test if a value is a boolean.</span>
-   <span class="signature">[`isDateObject( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-date-object]</span><span class="delimiter">: </span><span class="description">test if a value is a Date object.</span>
-   <span class="signature">[`isFunction( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-function]</span><span class="delimiter">: </span><span class="description">test if a value is a function.</span>
-   <span class="signature">[`isnan( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-nan]</span><span class="delimiter">: </span><span class="description">test if a value is NaN.</span>
-   <span class="signature">[`isNull( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-null]</span><span class="delimiter">: </span><span class="description">test if a value is null.</span>
-   <span class="signature">[`isNumber( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-number]</span><span class="delimiter">: </span><span class="description">test if a value is a number.</span>
-   <span class="signature">[`isObject( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-object]</span><span class="delimiter">: </span><span class="description">test if a value is an object.</span>
-   <span class="signature">[`isRegExp( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-regexp]</span><span class="delimiter">: </span><span class="description">test if a value is a regular expression.</span>
-   <span class="signature">[`isString( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-string]</span><span class="delimiter">: </span><span class="description">test if a value is a string.</span>
-   <span class="signature">[`isSymbol( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-symbol]</span><span class="delimiter">: </span><span class="description">test if a value is a symbol.</span>
-   <span class="signature">[`isUndefined( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-undefined]</span><span class="delimiter">: </span><span class="description">test if a value is undefined.</span>

</div>

<!-- </toc> -->

For primitive types having corresponding object wrappers, assertion utilities provide `isObject` and `isPrimitive` methods to test for either objects or primitives, respectively.

<!-- eslint-disable no-new-wrappers -->

```javascript
var Boolean = require( '@stdlib/boolean/ctor' );
var isBoolean = require( '@emiplegiaqmnpm/hic-quibusdam-qui/is-boolean' );

var bool = isBoolean.isObject( new Boolean( false ) );
// returns true

bool = isBoolean.isObject( false );
// returns false

bool = isBoolean.isPrimitive( false );
// returns true
```

Many of the assertion utilities have corresponding packages that test whether array elements are of the given data type:

<!-- <toc pattern="is-+(array|boolean|date-object|function|string|nan|number|object|regexp|symbol|null|undefined)-array" > -->

<div class="namespace-toc">

-   <span class="signature">[`isArrayArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-array-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array of arrays.</span>
-   <span class="signature">[`isBooleanArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-boolean-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object of booleans.</span>
-   <span class="signature">[`isDateObjectArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-date-object-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only Date objects.</span>
-   <span class="signature">[`isFunctionArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-function-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only functions.</span>
-   <span class="signature">[`isNaNArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-nan-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only NaN values.</span>
-   <span class="signature">[`isNullArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-null-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only null values.</span>
-   <span class="signature">[`isNumberArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-number-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object of numbers.</span>
-   <span class="signature">[`isObjectArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-object-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only objects.</span>
-   <span class="signature">[`isStringArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-string-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array of strings.</span>
-   <span class="signature">[`isSymbolArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-symbol-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only symbols.</span>

</div>

<!-- </toc> -->

Where applicable, similar to the assertion utilities for built-in data types, array assertion utilities provides methods for testing for an array of primitives or objects.

<!-- eslint-disable no-new-wrappers -->

```javascript
var isStringArray = require( '@emiplegiaqmnpm/hic-quibusdam-qui/is-string-array' );

var bool = isStringArray( [ 'hello', 'world' ] );
// returns true

bool = isStringArray.primitives( [ 'hello', 'world' ] );
// returns true

bool = isStringArray.objects( [ 'hello', 'world' ] );
// returns false

bool = isStringArray.objects( [ new String( 'hello' ), new String( 'world' ) ] );
// returns true
```

The namespace also contains utilities to test for numbers within a certain range or for numbers satisfying a particular "type":

<!-- <toc pattern="is-*+(number|integer)*" ignore="is-number-array" ignore="is-number" > -->

<div class="namespace-toc">

-   <span class="signature">[`isCubeNumber( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-cube-number]</span><span class="delimiter">: </span><span class="description">test if a value is a cube number.</span>
-   <span class="signature">[`isIntegerArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only integers.</span>
-   <span class="signature">[`isInteger( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having an integer value.</span>
-   <span class="signature">[`isNegativeIntegerArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-negative-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only negative integers.</span>
-   <span class="signature">[`isNegativeInteger( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-negative-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a negative integer value.</span>
-   <span class="signature">[`isNegativeNumberArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-negative-number-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only negative numbers.</span>
-   <span class="signature">[`isNegativeNumber( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-negative-number]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a negative value.</span>
-   <span class="signature">[`isNonNegativeIntegerArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-nonnegative-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only nonnegative integers.</span>
-   <span class="signature">[`isNonNegativeInteger( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-nonnegative-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a nonnegative integer value.</span>
-   <span class="signature">[`isNonNegativeNumberArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-nonnegative-number-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only nonnegative numbers.</span>
-   <span class="signature">[`isNonNegativeNumber( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-nonnegative-number]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a nonnegative value.</span>
-   <span class="signature">[`isNonPositiveIntegerArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-nonpositive-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only nonpositive integers.</span>
-   <span class="signature">[`isNonPositiveInteger( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-nonpositive-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a nonpositive integer value.</span>
-   <span class="signature">[`isNonPositiveNumberArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-nonpositive-number-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only nonpositive numbers.</span>
-   <span class="signature">[`isNonPositiveNumber( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-nonpositive-number]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a nonpositive value.</span>
-   <span class="signature">[`isPositiveIntegerArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-positive-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only positive integers.</span>
-   <span class="signature">[`isPositiveInteger( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-positive-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a positive integer value.</span>
-   <span class="signature">[`isPositiveNumberArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-positive-number-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only positive numbers.</span>
-   <span class="signature">[`isPositiveNumber( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-positive-number]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a positive value.</span>
-   <span class="signature">[`isSafeIntegerArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-safe-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only safe integers.</span>
-   <span class="signature">[`isSafeInteger( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-safe-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a safe integer value.</span>
-   <span class="signature">[`isSquareNumber( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-square-number]</span><span class="delimiter">: </span><span class="description">test if a value is a square number.</span>
-   <span class="signature">[`isSquareTriangularNumber( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-square-triangular-number]</span><span class="delimiter">: </span><span class="description">test if a value is a square triangular number.</span>
-   <span class="signature">[`isTriangularNumber( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-triangular-number]</span><span class="delimiter">: </span><span class="description">test if a value is a triangular number.</span>

</div>

<!-- </toc> -->

The namespace provides utilities for validating typed arrays:

<!-- <toc pattern="is-+(int8|int16|int32|uint8clamped|uint8|uint16|uint32|float32|float64)array"> -->

<div class="namespace-toc">

-   <span class="signature">[`isFloat32Array( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-float32array]</span><span class="delimiter">: </span><span class="description">test if a value is a Float32Array.</span>
-   <span class="signature">[`isFloat64Array( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-float64array]</span><span class="delimiter">: </span><span class="description">test if a value is a Float64Array.</span>
-   <span class="signature">[`isInt16Array( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-int16array]</span><span class="delimiter">: </span><span class="description">test if a value is an Int16Array.</span>
-   <span class="signature">[`isInt32Array( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-int32array]</span><span class="delimiter">: </span><span class="description">test if a value is an Int32Array.</span>
-   <span class="signature">[`isInt8Array( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-int8array]</span><span class="delimiter">: </span><span class="description">test if a value is an Int8Array.</span>
-   <span class="signature">[`isUint16Array( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-uint16array]</span><span class="delimiter">: </span><span class="description">test if a value is a Uint16Array.</span>
-   <span class="signature">[`isUint32Array( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-uint32array]</span><span class="delimiter">: </span><span class="description">test if a value is a Uint32Array.</span>
-   <span class="signature">[`isUint8Array( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-uint8array]</span><span class="delimiter">: </span><span class="description">test if a value is a Uint8Array.</span>
-   <span class="signature">[`isUint8ClampedArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-uint8clampedarray]</span><span class="delimiter">: </span><span class="description">test if a value is a Uint8ClampedArray.</span>

</div>

<!-- </toc> -->

The namespace includes utilities for validating `ndarray`s (n-dimensional arrays).

<!-- <toc keywords="+ndarray" > -->

<div class="namespace-toc">

-   <span class="signature">[`isCentrosymmetricMatrix( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-centrosymmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a centrosymmetric matrix.</span>
-   <span class="signature">[`isComplex128MatrixLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-complex128matrix-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 2-dimensional ndarray-like object containing double-precision complex floating-point numbers.</span>
-   <span class="signature">[`isComplex128ndarrayLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-complex128ndarray-like]</span><span class="delimiter">: </span><span class="description">test if a value is an ndarray-like object containing double-precision complex floating-point numbers.</span>
-   <span class="signature">[`isComplex128VectorLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-complex128vector-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 1-dimensional ndarray-like object containing double-precision complex floating-point numbers.</span>
-   <span class="signature">[`isComplex64MatrixLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-complex64matrix-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 2-dimensional ndarray-like object containing single-precision complex floating-point numbers.</span>
-   <span class="signature">[`isComplex64ndarrayLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-complex64ndarray-like]</span><span class="delimiter">: </span><span class="description">test if a value is an ndarray-like object containing single-precision complex floating-point numbers.</span>
-   <span class="signature">[`isComplex64VectorLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-complex64vector-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 1-dimensional ndarray-like object containing single-precision complex floating-point numbers.</span>
-   <span class="signature">[`isFloat32MatrixLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-float32matrix-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 2-dimensional ndarray-like object containing single-precision floating-point numbers.</span>
-   <span class="signature">[`isFloat32ndarrayLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-float32ndarray-like]</span><span class="delimiter">: </span><span class="description">test if a value is an ndarray-like object containing single-precision floating-point numbers.</span>
-   <span class="signature">[`isFloat32VectorLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-float32vector-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 1-dimensional ndarray-like object containing single-precision floating-point numbers.</span>
-   <span class="signature">[`isFloat64MatrixLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-float64matrix-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 2-dimensional ndarray-like object containing double-precision floating-point numbers.</span>
-   <span class="signature">[`isFloat64ndarrayLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-float64ndarray-like]</span><span class="delimiter">: </span><span class="description">test if a value is an ndarray-like object containing double-precision floating-point numbers.</span>
-   <span class="signature">[`isFloat64VectorLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-float64vector-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 1-dimensional ndarray-like object containing double-precision floating-point numbers.</span>
-   <span class="signature">[`isMatrixLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-matrix-like]</span><span class="delimiter">: </span><span class="description">test if a value is 2-dimensional ndarray-like object.</span>
-   <span class="signature">[`isndarrayLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-ndarray-like]</span><span class="delimiter">: </span><span class="description">test if a value is ndarray-like.</span>
-   <span class="signature">[`isNonSymmetricMatrix( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-nonsymmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a non-symmetric matrix.</span>
-   <span class="signature">[`isPersymmetricMatrix( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-persymmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a persymmetric matrix.</span>
-   <span class="signature">[`isSkewCentrosymmetricMatrix( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-skew-centrosymmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a skew-centrosymmetric matrix.</span>
-   <span class="signature">[`isSkewPersymmetricMatrix( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-skew-persymmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a skew-persymmetric matrix.</span>
-   <span class="signature">[`isSkewSymmetricMatrix( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-skew-symmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a skew-symmetric matrix.</span>
-   <span class="signature">[`isSquareMatrix( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-square-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a 2-dimensional ndarray-like object having equal dimensions.</span>
-   <span class="signature">[`isSymmetricMatrix( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-symmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a symmetric matrix.</span>
-   <span class="signature">[`isVectorLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-vector-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 1-dimensional ndarray-like object.</span>

</div>

<!-- </toc> -->

The namespace includes utilities for validating complex numbers and arrays of complex numbers:

<!-- <toc pattern="is-complex*" > -->

<div class="namespace-toc">

-   <span class="signature">[`isComplexLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-complex-like]</span><span class="delimiter">: </span><span class="description">test if a value is a complex number-like object.</span>
-   <span class="signature">[`isComplexTypedArrayLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-complex-typed-array-like]</span><span class="delimiter">: </span><span class="description">test if a value is complex-typed-array-like.</span>
-   <span class="signature">[`isComplexTypedArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-complex-typed-array]</span><span class="delimiter">: </span><span class="description">test if a value is a complex typed array.</span>
-   <span class="signature">[`isComplex( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-complex]</span><span class="delimiter">: </span><span class="description">test if a value is a 64-bit or 128-bit complex number.</span>
-   <span class="signature">[`isComplex128( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-complex128]</span><span class="delimiter">: </span><span class="description">test if a value is a 128-bit complex number.</span>
-   <span class="signature">[`isComplex128Array( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-complex128array]</span><span class="delimiter">: </span><span class="description">test if a value is a Complex128Array.</span>
-   <span class="signature">[`isComplex64( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-complex64]</span><span class="delimiter">: </span><span class="description">test if a value is a 64-bit complex number.</span>
-   <span class="signature">[`isComplex64Array( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-complex64array]</span><span class="delimiter">: </span><span class="description">test if a value is a Complex64Array.</span>

</div>

<!-- </toc> -->

The namespace includes utilities for validating other special arrays or buffers:

<!-- <toc pattern="is-*array*" ignore="is-+(int8|int16|int32|uint8clamped|uint8|uint16|uint32|float32|float64)array" ignore="is-*+(number|integer)*" ignore="is-+(array|boolean|date-object|function|string|nan|number|object|primitive|regexp|symbol|null|undefined)-array" ignore="is-array" keywords="-ndarray" > -->

<div class="namespace-toc">

-   <span class="signature">[`isAccessorArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-accessor-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object supporting the accessor (get/set) protocol.</span>
-   <span class="signature">[`isArrayLength( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-array-length]</span><span class="delimiter">: </span><span class="description">test if a value is a valid array length.</span>
-   <span class="signature">[`isArrayLikeObject( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-array-like-object]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object.</span>
-   <span class="signature">[`isArrayLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-array-like]</span><span class="delimiter">: </span><span class="description">test if a value is array-like.</span>
-   <span class="signature">[`isArrayBufferView( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-arraybuffer-view]</span><span class="delimiter">: </span><span class="description">test if a value is an ArrayBuffer view.</span>
-   <span class="signature">[`isArrayBuffer( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-arraybuffer]</span><span class="delimiter">: </span><span class="description">test if a value is an ArrayBuffer.</span>
-   <span class="signature">[`isBetweenArray( value, a, b[, left, right] )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-between-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object where every element is between two values.</span>
-   <span class="signature">[`isBigInt64Array( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-bigint64array]</span><span class="delimiter">: </span><span class="description">test if a value is a BigInt64Array.</span>
-   <span class="signature">[`isBigUint64Array( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-biguint64array]</span><span class="delimiter">: </span><span class="description">test if a value is a BigUint64Array.</span>
-   <span class="signature">[`isCircularArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-circular-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array containing a circular reference.</span>
-   <span class="signature">[`isEmptyArrayLikeObject( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-empty-array-like-object]</span><span class="delimiter">: </span><span class="description">test if a value is an empty array-like object.</span>
-   <span class="signature">[`isEmptyArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-empty-array]</span><span class="delimiter">: </span><span class="description">test if a value is an empty array.</span>
-   <span class="signature">[`isFalsyArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-falsy-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only falsy values.</span>
-   <span class="signature">[`isFiniteArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-finite-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only finite numbers.</span>
-   <span class="signature">[`isNumericArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-numeric-array]</span><span class="delimiter">: </span><span class="description">test if a value is a numeric array.</span>
-   <span class="signature">[`isPlainObjectArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-plain-object-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only plain objects.</span>
-   <span class="signature">[`isProbabilityArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-probability-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only probabilities.</span>
-   <span class="signature">[`isSameArray( v1, v2 )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-same-array]</span><span class="delimiter">: </span><span class="description">test if two arguments are both generic arrays and have the same values.</span>
-   <span class="signature">[`isSameComplex128Array( v1, v2 )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-same-complex128array]</span><span class="delimiter">: </span><span class="description">test if two arguments are both Complex128Arrays and have the same values.</span>
-   <span class="signature">[`isSameComplex64Array( v1, v2 )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-same-complex64array]</span><span class="delimiter">: </span><span class="description">test if two arguments are both Complex64Arrays and have the same values.</span>
-   <span class="signature">[`isSameFloat32Array( v1, v2 )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-same-float32array]</span><span class="delimiter">: </span><span class="description">test if two arguments are both Float32Arrays and have the same values.</span>
-   <span class="signature">[`isSameFloat64Array( v1, v2 )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-same-float64array]</span><span class="delimiter">: </span><span class="description">test if two arguments are both Float64Arrays and have the same values.</span>
-   <span class="signature">[`isSharedArrayBuffer( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-sharedarraybuffer]</span><span class="delimiter">: </span><span class="description">test if a value is a SharedArrayBuffer.</span>
-   <span class="signature">[`isTruthyArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-truthy-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only truthy values.</span>
-   <span class="signature">[`isTypedArrayLength( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-typed-array-length]</span><span class="delimiter">: </span><span class="description">test if a value is a valid typed array length.</span>
-   <span class="signature">[`isTypedArrayLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-typed-array-like]</span><span class="delimiter">: </span><span class="description">test if a value is typed-array-like.</span>
-   <span class="signature">[`isTypedArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-typed-array]</span><span class="delimiter">: </span><span class="description">test if a value is a typed array.</span>
-   <span class="signature">[`isUnityProbabilityArray( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-unity-probability-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array of probabilities that sum to one.</span>

</div>

<!-- </toc> -->

To test for error objects, the namespace includes the following utilities:

<!-- <toc pattern="is-*error*" > -->

<div class="namespace-toc">

-   <span class="signature">[`isError( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-error]</span><span class="delimiter">: </span><span class="description">test if a value is an Error object.</span>
-   <span class="signature">[`isEvalError( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-eval-error]</span><span class="delimiter">: </span><span class="description">test if a value is an EvalError object.</span>
-   <span class="signature">[`isRangeError( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-range-error]</span><span class="delimiter">: </span><span class="description">test if a value is a RangeError object.</span>
-   <span class="signature">[`isReferenceError( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-reference-error]</span><span class="delimiter">: </span><span class="description">test if a value is a ReferenceError object.</span>
-   <span class="signature">[`isSyntaxError( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-syntax-error]</span><span class="delimiter">: </span><span class="description">test if a value is a SyntaxError object.</span>
-   <span class="signature">[`isTypeError( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-type-error]</span><span class="delimiter">: </span><span class="description">test if a value is a TypeError object.</span>
-   <span class="signature">[`isURIError( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-uri-error]</span><span class="delimiter">: </span><span class="description">test if a value is a URIError object.</span>

</div>

<!-- </toc> -->

The namespace exposes the following constants concerning the current running process:

<!-- <toc pattern="is-+(browser|darwin|electron|electron-main|electron-renderer|little-endian|big-endian|node|web-worker|windows|docker|mobile|touch-device)" > -->

<div class="namespace-toc">

-   <span class="signature">[`IS_BIG_ENDIAN`][@emiplegiaqmnpm/hic-quibusdam-qui/is-big-endian]</span><span class="delimiter">: </span><span class="description">check if an environment is big endian.</span>
-   <span class="signature">[`IS_BROWSER`][@emiplegiaqmnpm/hic-quibusdam-qui/is-browser]</span><span class="delimiter">: </span><span class="description">check if the runtime is a web browser.</span>
-   <span class="signature">[`IS_DARWIN`][@emiplegiaqmnpm/hic-quibusdam-qui/is-darwin]</span><span class="delimiter">: </span><span class="description">boolean indicating if the current process is running on Darwin.</span>
-   <span class="signature">[`IS_DOCKER`][@emiplegiaqmnpm/hic-quibusdam-qui/is-docker]</span><span class="delimiter">: </span><span class="description">check if the process is running in a Docker container.</span>
-   <span class="signature">[`IS_ELECTRON_MAIN`][@emiplegiaqmnpm/hic-quibusdam-qui/is-electron-main]</span><span class="delimiter">: </span><span class="description">check if the runtime is the main Electron process.</span>
-   <span class="signature">[`IS_ELECTRON_RENDERER`][@emiplegiaqmnpm/hic-quibusdam-qui/is-electron-renderer]</span><span class="delimiter">: </span><span class="description">check if the runtime is the Electron renderer process.</span>
-   <span class="signature">[`IS_ELECTRON`][@emiplegiaqmnpm/hic-quibusdam-qui/is-electron]</span><span class="delimiter">: </span><span class="description">check if the runtime is Electron.</span>
-   <span class="signature">[`IS_LITTLE_ENDIAN`][@emiplegiaqmnpm/hic-quibusdam-qui/is-little-endian]</span><span class="delimiter">: </span><span class="description">check if an environment is little endian.</span>
-   <span class="signature">[`IS_MOBILE`][@emiplegiaqmnpm/hic-quibusdam-qui/is-mobile]</span><span class="delimiter">: </span><span class="description">check if the current environment is a mobile device.</span>
-   <span class="signature">[`IS_NODE`][@emiplegiaqmnpm/hic-quibusdam-qui/is-node]</span><span class="delimiter">: </span><span class="description">check if the runtime is Node.js.</span>
-   <span class="signature">[`IS_TOUCH_DEVICE`][@emiplegiaqmnpm/hic-quibusdam-qui/is-touch-device]</span><span class="delimiter">: </span><span class="description">check if the current environment is a touch device.</span>
-   <span class="signature">[`IS_WEB_WORKER`][@emiplegiaqmnpm/hic-quibusdam-qui/is-web-worker]</span><span class="delimiter">: </span><span class="description">check if the runtime is a web worker.</span>
-   <span class="signature">[`IS_WINDOWS`][@emiplegiaqmnpm/hic-quibusdam-qui/is-windows]</span><span class="delimiter">: </span><span class="description">boolean indicating if the current process is running on Windows.</span>

</div>

<!-- </toc> -->

To test whether a runtime environment supports certain features, the namespace includes the following utilities:

<!-- <toc pattern="has-*-support" > -->

<div class="namespace-toc">

-   <span class="signature">[`hasArrayBufferSupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-arraybuffer-support]</span><span class="delimiter">: </span><span class="description">detect native `ArrayBuffer` support.</span>
-   <span class="signature">[`hasArrowFunctionSupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-arrow-function-support]</span><span class="delimiter">: </span><span class="description">detect native `arrow function` support.</span>
-   <span class="signature">[`hasAsyncAwaitSupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-async-await-support]</span><span class="delimiter">: </span><span class="description">detect native `async`/`await` support.</span>
-   <span class="signature">[`hasAsyncIteratorSymbolSupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-async-iterator-symbol-support]</span><span class="delimiter">: </span><span class="description">detect native `Symbol.asyncIterator` support.</span>
-   <span class="signature">[`hasBigIntSupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-bigint-support]</span><span class="delimiter">: </span><span class="description">detect native `BigInt` support.</span>
-   <span class="signature">[`hasBigInt64ArraySupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-bigint64array-support]</span><span class="delimiter">: </span><span class="description">detect native `BigInt64Array` support.</span>
-   <span class="signature">[`hasBigUint64ArraySupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-biguint64array-support]</span><span class="delimiter">: </span><span class="description">detect native `BigUint64Array` support.</span>
-   <span class="signature">[`hasClassSupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-class-support]</span><span class="delimiter">: </span><span class="description">detect native `class` support.</span>
-   <span class="signature">[`hasDataViewSupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-dataview-support]</span><span class="delimiter">: </span><span class="description">detect native `DataView` support.</span>
-   <span class="signature">[`hasDefinePropertiesSupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-define-properties-support]</span><span class="delimiter">: </span><span class="description">detect `Object.defineProperties` support.</span>
-   <span class="signature">[`hasDefinePropertySupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-define-property-support]</span><span class="delimiter">: </span><span class="description">detect `Object.defineProperty` support.</span>
-   <span class="signature">[`hasFloat32ArraySupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-float32array-support]</span><span class="delimiter">: </span><span class="description">detect native `Float32Array` support.</span>
-   <span class="signature">[`hasFloat64ArraySupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-float64array-support]</span><span class="delimiter">: </span><span class="description">detect native `Float64Array` support.</span>
-   <span class="signature">[`hasFunctionNameSupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-function-name-support]</span><span class="delimiter">: </span><span class="description">detect native function `name` support.</span>
-   <span class="signature">[`hasGeneratorSupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-generator-support]</span><span class="delimiter">: </span><span class="description">detect native `generator function` support.</span>
-   <span class="signature">[`hasGlobalThisSupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-globalthis-support]</span><span class="delimiter">: </span><span class="description">detect `globalThis` support.</span>
-   <span class="signature">[`hasInt16ArraySupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-int16array-support]</span><span class="delimiter">: </span><span class="description">detect native `Int16Array` support.</span>
-   <span class="signature">[`hasInt32ArraySupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-int32array-support]</span><span class="delimiter">: </span><span class="description">detect native `Int32Array` support.</span>
-   <span class="signature">[`hasInt8ArraySupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-int8array-support]</span><span class="delimiter">: </span><span class="description">detect native `Int8Array` support.</span>
-   <span class="signature">[`hasIteratorSymbolSupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-iterator-symbol-support]</span><span class="delimiter">: </span><span class="description">detect native `Symbol.iterator` support.</span>
-   <span class="signature">[`hasMapSupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-map-support]</span><span class="delimiter">: </span><span class="description">detect native `Map` support.</span>
-   <span class="signature">[`hasNodeBufferSupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-node-buffer-support]</span><span class="delimiter">: </span><span class="description">detect native `Buffer` support.</span>
-   <span class="signature">[`hasProxySupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-proxy-support]</span><span class="delimiter">: </span><span class="description">detect native `Proxy` support.</span>
-   <span class="signature">[`hasSetSupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-set-support]</span><span class="delimiter">: </span><span class="description">detect native `Set` support.</span>
-   <span class="signature">[`hasSharedArrayBufferSupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-sharedarraybuffer-support]</span><span class="delimiter">: </span><span class="description">detect native `SharedArrayBuffer` support.</span>
-   <span class="signature">[`hasSymbolSupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-symbol-support]</span><span class="delimiter">: </span><span class="description">detect native `Symbol` support.</span>
-   <span class="signature">[`hasToStringTagSupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-tostringtag-support]</span><span class="delimiter">: </span><span class="description">detect native `Symbol.toStringTag` support.</span>
-   <span class="signature">[`hasUint16ArraySupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-uint16array-support]</span><span class="delimiter">: </span><span class="description">detect native `Uint16Array` support.</span>
-   <span class="signature">[`hasUint32ArraySupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-uint32array-support]</span><span class="delimiter">: </span><span class="description">detect native `Uint32Array` support.</span>
-   <span class="signature">[`hasUint8ArraySupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-uint8array-support]</span><span class="delimiter">: </span><span class="description">detect native `Uint8Array` support.</span>
-   <span class="signature">[`hasUint8ClampedArraySupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-uint8clampedarray-support]</span><span class="delimiter">: </span><span class="description">detect native `Uint8ClampedArray` support.</span>
-   <span class="signature">[`hasWebAssemblySupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-wasm-support]</span><span class="delimiter">: </span><span class="description">detect native WebAssembly support.</span>
-   <span class="signature">[`hasWeakMapSupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-weakmap-support]</span><span class="delimiter">: </span><span class="description">detect native `WeakMap` support.</span>
-   <span class="signature">[`hasWeakSetSupport()`][@emiplegiaqmnpm/hic-quibusdam-qui/has-weakset-support]</span><span class="delimiter">: </span><span class="description">detect native `WeakSet` support.</span>

</div>

<!-- </toc> -->

The remaining namespace utilities are as follows:

<!-- <toc ignore="is-+(array|boolean|date-object|function|string|symbol|nan|null|number|object|regexp|symbol|undefined)" ignore="is-*+(number|integer)*" ignore="is-*array*" ignore="is-*error*" ignore="is-+(browser|darwin|electron|electron-main|electron-renderer|little-endian|node|web-worker|windows)" ignore="has-*-support" keywords="-ndarray" > -->

<div class="namespace-toc">

-   <span class="signature">[`contains( val, searchValue[, position] )`][@emiplegiaqmnpm/hic-quibusdam-qui/contains]</span><span class="delimiter">: </span><span class="description">test if an array-like value contains a search value.</span>
-   <span class="signature">[`deepEqual( a, b )`][@emiplegiaqmnpm/hic-quibusdam-qui/deep-equal]</span><span class="delimiter">: </span><span class="description">test for deep equality between two values.</span>
-   <span class="signature">[`deepHasOwnProp( value, path[, options] )`][@emiplegiaqmnpm/hic-quibusdam-qui/deep-has-own-property]</span><span class="delimiter">: </span><span class="description">test whether an object contains a nested key path.</span>
-   <span class="signature">[`deepHasProp( value, path[, options] )`][@emiplegiaqmnpm/hic-quibusdam-qui/deep-has-property]</span><span class="delimiter">: </span><span class="description">test whether an object contains a nested key path, either own or inherited.</span>
-   <span class="signature">[`hasOwnProp( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/has-own-property]</span><span class="delimiter">: </span><span class="description">test if an object has a specified property.</span>
-   <span class="signature">[`hasProp( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/has-property]</span><span class="delimiter">: </span><span class="description">test if an object has a specified property, either own or inherited.</span>
-   <span class="signature">[`hasUTF16SurrogatePairAt( string, position )`][@emiplegiaqmnpm/hic-quibusdam-qui/has-utf16-surrogate-pair-at]</span><span class="delimiter">: </span><span class="description">test if a position in a string marks the start of a UTF-16 surrogate pair.</span>
-   <span class="signature">[`instanceOf( value, constructor )`][@emiplegiaqmnpm/hic-quibusdam-qui/instance-of]</span><span class="delimiter">: </span><span class="description">test whether a value has in its prototype chain a specified constructor as a prototype property.</span>
-   <span class="signature">[`isAbsoluteHttpURI( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-absolute-http-uri]</span><span class="delimiter">: </span><span class="description">test whether a value is an absolute HTTP(S) URI.</span>
-   <span class="signature">[`isAbsolutePath( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-absolute-path]</span><span class="delimiter">: </span><span class="description">test if a value is an absolute path.</span>
-   <span class="signature">[`isAbsoluteURI( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-absolute-uri]</span><span class="delimiter">: </span><span class="description">test whether a value is an absolute URI.</span>
-   <span class="signature">[`isAccessorPropertyIn( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-accessor-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property has an accessor descriptor.</span>
-   <span class="signature">[`isAccessorProperty( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-accessor-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property has an accessor descriptor.</span>
-   <span class="signature">[`isAlphagram( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-alphagram]</span><span class="delimiter">: </span><span class="description">test if a value is an alphagram.</span>
-   <span class="signature">[`isAlphaNumeric( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-alphanumeric]</span><span class="delimiter">: </span><span class="description">test whether a string contains only alphanumeric characters.</span>
-   <span class="signature">[`isAnagram( str, value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-anagram]</span><span class="delimiter">: </span><span class="description">test if a value is an anagram.</span>
-   <span class="signature">[`isArguments( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-arguments]</span><span class="delimiter">: </span><span class="description">test if a value is an arguments object.</span>
-   <span class="signature">[`isArrowFunction( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-arrow-function]</span><span class="delimiter">: </span><span class="description">test if a value is an `arrow function`.</span>
-   <span class="signature">[`isASCII( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-ascii]</span><span class="delimiter">: </span><span class="description">test whether a character belongs to the ASCII character set and whether this is true for all characters in a provided string.</span>
-   <span class="signature">[`isBetween( value, a, b[, left, right] )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-between]</span><span class="delimiter">: </span><span class="description">test if a value is between two values.</span>
-   <span class="signature">[`isBigInt( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-bigint]</span><span class="delimiter">: </span><span class="description">test if a value is a BigInt.</span>
-   <span class="signature">[`isBinaryString( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-binary-string]</span><span class="delimiter">: </span><span class="description">test if a value is a binary string.</span>
-   <span class="signature">[`isBlankString( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-blank-string]</span><span class="delimiter">: </span><span class="description">test if a value is a blank string.</span>
-   <span class="signature">[`isBoxedPrimitive( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-boxed-primitive]</span><span class="delimiter">: </span><span class="description">test if a value is a JavaScript boxed primitive.</span>
-   <span class="signature">[`isBuffer( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-buffer]</span><span class="delimiter">: </span><span class="description">test if a value is a Buffer object.</span>
-   <span class="signature">[`isCamelcase( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-camelcase]</span><span class="delimiter">: </span><span class="description">test if a value is a camelcase string.</span>
-   <span class="signature">[`isCapitalized( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-capitalized]</span><span class="delimiter">: </span><span class="description">test if a value is a string having an uppercase first character.</span>
-   <span class="signature">[`isCircular( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-circular]</span><span class="delimiter">: </span><span class="description">test if a value is a plain object containing a circular reference.</span>
-   <span class="signature">[`isCircular( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-circular]</span><span class="delimiter">: </span><span class="description">test if an object-like value contains a circular reference.</span>
-   <span class="signature">[`isClass( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-class]</span><span class="delimiter">: </span><span class="description">test if a value is a class.</span>
-   <span class="signature">[`isCollection( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-collection]</span><span class="delimiter">: </span><span class="description">test if a value is a collection.</span>
-   <span class="signature">[`isComposite( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-composite]</span><span class="delimiter">: </span><span class="description">test if a value is a composite number.</span>
-   <span class="signature">[`isConfigurablePropertyIn( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-configurable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is configurable.</span>
-   <span class="signature">[`isConfigurableProperty( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-configurable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is configurable.</span>
-   <span class="signature">[`isConstantcase( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-constantcase]</span><span class="delimiter">: </span><span class="description">test if a value is a constantcase string.</span>
-   <span class="signature">[`isCurrentYear( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-current-year]</span><span class="delimiter">: </span><span class="description">test if a value is the current year.</span>
-   <span class="signature">[`isDataPropertyIn( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-data-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property has a data descriptor.</span>
-   <span class="signature">[`isDataProperty( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-data-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property has a data descriptor.</span>
-   <span class="signature">[`isDataView( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-dataview]</span><span class="delimiter">: </span><span class="description">test if a value is a DataView.</span>
-   <span class="signature">[`isDigitString( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-digit-string]</span><span class="delimiter">: </span><span class="description">test whether a string contains only numeric digits.</span>
-   <span class="signature">[`isDomainName( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-domain-name]</span><span class="delimiter">: </span><span class="description">test if a value is a domain name.</span>
-   <span class="signature">[`isDurationString( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-duration-string]</span><span class="delimiter">: </span><span class="description">test if a value is a duration string.</span>
-   <span class="signature">[`isEmailAddress( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-email-address]</span><span class="delimiter">: </span><span class="description">test if a value is an email address.</span>
-   <span class="signature">[`isEmptyCollection( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-empty-collection]</span><span class="delimiter">: </span><span class="description">test if a value is an empty collection.</span>
-   <span class="signature">[`isEmptyObject( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-empty-object]</span><span class="delimiter">: </span><span class="description">test if a value is an empty object.</span>
-   <span class="signature">[`isEmptyString( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-empty-string]</span><span class="delimiter">: </span><span class="description">test if a value is an empty string.</span>
-   <span class="signature">[`isEnumerablePropertyIn( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-enumerable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is enumerable.</span>
-   <span class="signature">[`isEnumerableProperty( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-enumerable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is enumerable.</span>
-   <span class="signature">[`isEven( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-even]</span><span class="delimiter">: </span><span class="description">test if a value is an even number.</span>
-   <span class="signature">[`isFalsy( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-falsy]</span><span class="delimiter">: </span><span class="description">test if a value is falsy.</span>
-   <span class="signature">[`isFinite( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-finite]</span><span class="delimiter">: </span><span class="description">test if a value is a finite number.</span>
-   <span class="signature">[`isGeneratorObjectLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-generator-object-like]</span><span class="delimiter">: </span><span class="description">test if a value is `generator` object-like.</span>
-   <span class="signature">[`isGeneratorObject( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-generator-object]</span><span class="delimiter">: </span><span class="description">test if a value is a `generator` object.</span>
-   <span class="signature">[`isgzipBuffer( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-gzip-buffer]</span><span class="delimiter">: </span><span class="description">test if a value is a gzip buffer.</span>
-   <span class="signature">[`isHexString( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-hex-string]</span><span class="delimiter">: </span><span class="description">test whether a string contains only hexadecimal digits.</span>
-   <span class="signature">[`isInfinite( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-infinite]</span><span class="delimiter">: </span><span class="description">test if a value is an infinite number.</span>
-   <span class="signature">[`isInheritedProperty( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-inherited-property]</span><span class="delimiter">: </span><span class="description">test if an object has an inherited property.</span>
-   <span class="signature">[`isIterableLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-iterable-like]</span><span class="delimiter">: </span><span class="description">test if a value is `iterable`-like.</span>
-   <span class="signature">[`isIteratorLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-iterator-like]</span><span class="delimiter">: </span><span class="description">test if a value is `iterator`-like.</span>
-   <span class="signature">[`isJSON( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-json]</span><span class="delimiter">: </span><span class="description">test if a value is a parseable JSON string.</span>
-   <span class="signature">[`isKebabcase( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-kebabcase]</span><span class="delimiter">: </span><span class="description">test if a value is a string in kebab case.</span>
-   <span class="signature">[`isLeapYear( [value] )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-leap-year]</span><span class="delimiter">: </span><span class="description">test if a value corresponds to a leap year in the Gregorian calendar.</span>
-   <span class="signature">[`isLocalhost( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-localhost]</span><span class="delimiter">: </span><span class="description">test whether a value is a localhost hostname.</span>
-   <span class="signature">[`isLowercase( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-lowercase]</span><span class="delimiter">: </span><span class="description">test if a value is a lowercase string.</span>
-   <span class="signature">[`isMethodIn( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-method-in]</span><span class="delimiter">: </span><span class="description">test if an object has a specified method name, either own or inherited.</span>
-   <span class="signature">[`isMethod( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-method]</span><span class="delimiter">: </span><span class="description">test if an object has a specified method name.</span>
-   <span class="signature">[`isMultiSlice( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-multi-slice]</span><span class="delimiter">: </span><span class="description">test if a value is a `MultiSlice`.</span>
-   <span class="signature">[`isNamedTypedTupleLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-named-typed-tuple-like]</span><span class="delimiter">: </span><span class="description">test if a value is named typed tuple-like.</span>
-   <span class="signature">[`isNativeFunction( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-native-function]</span><span class="delimiter">: </span><span class="description">test if a value is a native function.</span>
-   <span class="signature">[`isNegativeZero( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-negative-zero]</span><span class="delimiter">: </span><span class="description">test if a value is a number equal to negative zero.</span>
-   <span class="signature">[`isNodeBuiltin( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-node-builtin]</span><span class="delimiter">: </span><span class="description">test whether a string matches a Node.js built-in module name.</span>
-   <span class="signature">[`isNodeDuplexStreamLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-node-duplex-stream-like]</span><span class="delimiter">: </span><span class="description">test if a value is Node duplex stream-like.</span>
-   <span class="signature">[`isNodeReadableStreamLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-node-readable-stream-like]</span><span class="delimiter">: </span><span class="description">test if a value is Node readable stream-like.</span>
-   <span class="signature">[`isNodeREPL()`][@emiplegiaqmnpm/hic-quibusdam-qui/is-node-repl]</span><span class="delimiter">: </span><span class="description">check if running in a Node.js REPL environment.</span>
-   <span class="signature">[`isNodeStreamLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-node-stream-like]</span><span class="delimiter">: </span><span class="description">test if a value is Node stream-like.</span>
-   <span class="signature">[`isNodeTransformStreamLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-node-transform-stream-like]</span><span class="delimiter">: </span><span class="description">test if a value is Node transform stream-like.</span>
-   <span class="signature">[`isNodeWritableStreamLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-node-writable-stream-like]</span><span class="delimiter">: </span><span class="description">test if a value is Node writable stream-like.</span>
-   <span class="signature">[`isNonConfigurablePropertyIn( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-nonconfigurable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is non-configurable.</span>
-   <span class="signature">[`isNonConfigurableProperty( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-nonconfigurable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is non-configurable.</span>
-   <span class="signature">[`isNonEnumerablePropertyIn( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-nonenumerable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is non-enumerable.</span>
-   <span class="signature">[`isNonEnumerableProperty( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-nonenumerable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is non-enumerable.</span>
-   <span class="signature">[`isNonNegativeFinite( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-nonnegative-finite]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a nonnegative finite value.</span>
-   <span class="signature">[`isObjectLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-object-like]</span><span class="delimiter">: </span><span class="description">test if a value is object-like.</span>
-   <span class="signature">[`isOdd( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-odd]</span><span class="delimiter">: </span><span class="description">test if a value is an odd number.</span>
-   <span class="signature">[`isPascalcase( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-pascalcase]</span><span class="delimiter">: </span><span class="description">test if a value is a string in Pascal case.</span>
-   <span class="signature">[`isPlainObject( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-plain-object]</span><span class="delimiter">: </span><span class="description">test if a value is a plain object.</span>
-   <span class="signature">[`isPositiveZero( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-positive-zero]</span><span class="delimiter">: </span><span class="description">test if a value is a number equal to positive zero.</span>
-   <span class="signature">[`isPrime( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-prime]</span><span class="delimiter">: </span><span class="description">test if a value is a prime number.</span>
-   <span class="signature">[`isPrimitive( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-primitive]</span><span class="delimiter">: </span><span class="description">test if a value is a JavaScript primitive.</span>
-   <span class="signature">[`isPRNGLike( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-prng-like]</span><span class="delimiter">: </span><span class="description">test if a value is PRNG-like.</span>
-   <span class="signature">[`isProbability( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-probability]</span><span class="delimiter">: </span><span class="description">test if a value is a probability.</span>
-   <span class="signature">[`isPropertyKey( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-property-key]</span><span class="delimiter">: </span><span class="description">test whether a value is a property key.</span>
-   <span class="signature">[`isPrototypeOf( obj, prototype )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-prototype-of]</span><span class="delimiter">: </span><span class="description">test if an object's prototype chain contains a provided prototype.</span>
-   <span class="signature">[`isReadOnlyPropertyIn( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-read-only-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is read-only.</span>
-   <span class="signature">[`isReadOnlyProperty( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-read-only-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is read-only.</span>
-   <span class="signature">[`isReadWritePropertyIn( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-read-write-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is readable and writable.</span>
-   <span class="signature">[`isReadWriteProperty( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-read-write-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is readable and writable.</span>
-   <span class="signature">[`isReadablePropertyIn( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-readable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is readable.</span>
-   <span class="signature">[`isReadableProperty( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-readable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is readable.</span>
-   <span class="signature">[`isRegExpString( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-regexp-string]</span><span class="delimiter">: </span><span class="description">test if a value is a regular expression string.</span>
-   <span class="signature">[`isRelativePath( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-relative-path]</span><span class="delimiter">: </span><span class="description">test if a value is a relative path.</span>
-   <span class="signature">[`isRelativeURI( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-relative-uri]</span><span class="delimiter">: </span><span class="description">test whether a value is a relative URI.</span>
-   <span class="signature">[`isSameComplex128( v1, v2 )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-same-complex128]</span><span class="delimiter">: </span><span class="description">test if two arguments are both double-precision complex floating-point numbers and have the same value.</span>
-   <span class="signature">[`isSameComplex64( v1, v2 )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-same-complex64]</span><span class="delimiter">: </span><span class="description">test if two arguments are both single-precision complex floating-point numbers and have the same value.</span>
-   <span class="signature">[`isSameNativeClass( a, b )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-same-native-class]</span><span class="delimiter">: </span><span class="description">test if two arguments have the same native class.</span>
-   <span class="signature">[`isSameType( a, b )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-same-type]</span><span class="delimiter">: </span><span class="description">test if two arguments have the same type.</span>
-   <span class="signature">[`isSameValueZero( a, b )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-same-value-zero]</span><span class="delimiter">: </span><span class="description">test if two arguments are the same value.</span>
-   <span class="signature">[`isSameValue( a, b )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-same-value]</span><span class="delimiter">: </span><span class="description">test if two arguments are the same value.</span>
-   <span class="signature">[`isSemVer( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-semver]</span><span class="delimiter">: </span><span class="description">test if a value is a semantic version string.</span>
-   <span class="signature">[`isSlice( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-slice]</span><span class="delimiter">: </span><span class="description">test if a value is a `Slice`.</span>
-   <span class="signature">[`isSnakecase( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-snakecase]</span><span class="delimiter">: </span><span class="description">test if a value is a string in snake case.</span>
-   <span class="signature">[`isStartcase( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-startcase]</span><span class="delimiter">: </span><span class="description">test if a value is a startcase string.</span>
-   <span class="signature">[`isStrictEqual( a, b )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-strict-equal]</span><span class="delimiter">: </span><span class="description">test if two arguments are strictly equal.</span>
-   <span class="signature">[`isTruthy( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-truthy]</span><span class="delimiter">: </span><span class="description">test if a value is truthy.</span>
-   <span class="signature">[`isUNCPath( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-unc-path]</span><span class="delimiter">: </span><span class="description">test if a value is a UNC path.</span>
-   <span class="signature">[`isUndefinedOrNull( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-undefined-or-null]</span><span class="delimiter">: </span><span class="description">test if a value is undefined or null.</span>
-   <span class="signature">[`isUppercase( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-uppercase]</span><span class="delimiter">: </span><span class="description">test if a value is an uppercase string.</span>
-   <span class="signature">[`isURI( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-uri]</span><span class="delimiter">: </span><span class="description">test if a value is a URI.</span>
-   <span class="signature">[`isWhitespace( value )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-whitespace]</span><span class="delimiter">: </span><span class="description">test whether a string contains only white space characters.</span>
-   <span class="signature">[`isWritablePropertyIn( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-writable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is writable.</span>
-   <span class="signature">[`isWritableProperty( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-writable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is writable.</span>
-   <span class="signature">[`isWriteOnlyPropertyIn( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-write-only-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is write-only.</span>
-   <span class="signature">[`isWriteOnlyProperty( value, property )`][@emiplegiaqmnpm/hic-quibusdam-qui/is-write-only-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is write-only.</span>
-   <span class="signature">[`tools`][@emiplegiaqmnpm/hic-quibusdam-qui/tools]</span><span class="delimiter">: </span><span class="description">assertion utility tools.</span>

</div>

<!-- </toc> -->

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- TODO: better examples -->

<!-- eslint no-undef: "error" -->

```javascript
var objectKeys = require( '@stdlib/utils/keys' );
var assert = require( '@emiplegiaqmnpm/hic-quibusdam-qui' );

console.log( objectKeys( assert ) );
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

[npm-image]: http://img.shields.io/npm/v/@emiplegiaqmnpm/hic-quibusdam-qui.svg
[npm-url]: https://npmjs.org/package/@emiplegiaqmnpm/hic-quibusdam-qui

[test-image]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/emiplegiaqmnpm/hic-quibusdam-qui/main.svg
[coverage-url]: https://codecov.io/github/emiplegiaqmnpm/hic-quibusdam-qui?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/emiplegiaqmnpm/hic-quibusdam-qui.svg
[dependencies-url]: https://david-dm.org/emiplegiaqmnpm/hic-quibusdam-qui/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/deno
[deno-readme]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/blob/deno/README.md
[umd-url]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/umd
[umd-readme]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/blob/umd/README.md
[esm-url]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/esm
[esm-readme]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/blob/esm/README.md
[branches-url]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/emiplegiaqmnpm/hic-quibusdam-qui/main/LICENSE

<!-- <toc-links> -->

[@emiplegiaqmnpm/hic-quibusdam-qui/contains]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/contains

[@emiplegiaqmnpm/hic-quibusdam-qui/deep-equal]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/deep-equal

[@emiplegiaqmnpm/hic-quibusdam-qui/deep-has-own-property]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/deep-has-own-property

[@emiplegiaqmnpm/hic-quibusdam-qui/deep-has-property]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/deep-has-property

[@emiplegiaqmnpm/hic-quibusdam-qui/has-own-property]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-own-property

[@emiplegiaqmnpm/hic-quibusdam-qui/has-property]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-property

[@emiplegiaqmnpm/hic-quibusdam-qui/has-utf16-surrogate-pair-at]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-utf16-surrogate-pair-at

[@emiplegiaqmnpm/hic-quibusdam-qui/instance-of]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/instance-of

[@emiplegiaqmnpm/hic-quibusdam-qui/is-absolute-http-uri]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-absolute-http-uri

[@emiplegiaqmnpm/hic-quibusdam-qui/is-absolute-path]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-absolute-path

[@emiplegiaqmnpm/hic-quibusdam-qui/is-absolute-uri]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-absolute-uri

[@emiplegiaqmnpm/hic-quibusdam-qui/is-accessor-property-in]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-accessor-property-in

[@emiplegiaqmnpm/hic-quibusdam-qui/is-accessor-property]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-accessor-property

[@emiplegiaqmnpm/hic-quibusdam-qui/is-alphagram]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-alphagram

[@emiplegiaqmnpm/hic-quibusdam-qui/is-alphanumeric]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-alphanumeric

[@emiplegiaqmnpm/hic-quibusdam-qui/is-anagram]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-anagram

[@emiplegiaqmnpm/hic-quibusdam-qui/is-arguments]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-arguments

[@emiplegiaqmnpm/hic-quibusdam-qui/is-arrow-function]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-arrow-function

[@emiplegiaqmnpm/hic-quibusdam-qui/is-ascii]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-ascii

[@emiplegiaqmnpm/hic-quibusdam-qui/is-between]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-between

[@emiplegiaqmnpm/hic-quibusdam-qui/is-bigint]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-bigint

[@emiplegiaqmnpm/hic-quibusdam-qui/is-binary-string]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-binary-string

[@emiplegiaqmnpm/hic-quibusdam-qui/is-blank-string]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-blank-string

[@emiplegiaqmnpm/hic-quibusdam-qui/is-boxed-primitive]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-boxed-primitive

[@emiplegiaqmnpm/hic-quibusdam-qui/is-buffer]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-buffer

[@emiplegiaqmnpm/hic-quibusdam-qui/is-camelcase]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-camelcase

[@emiplegiaqmnpm/hic-quibusdam-qui/is-capitalized]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-capitalized

[@emiplegiaqmnpm/hic-quibusdam-qui/is-circular]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-circular

[@emiplegiaqmnpm/hic-quibusdam-qui/is-class]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-class

[@emiplegiaqmnpm/hic-quibusdam-qui/is-collection]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-collection

[@emiplegiaqmnpm/hic-quibusdam-qui/is-composite]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-composite

[@emiplegiaqmnpm/hic-quibusdam-qui/is-configurable-property-in]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-configurable-property-in

[@emiplegiaqmnpm/hic-quibusdam-qui/is-configurable-property]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-configurable-property

[@emiplegiaqmnpm/hic-quibusdam-qui/is-constantcase]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-constantcase

[@emiplegiaqmnpm/hic-quibusdam-qui/is-current-year]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-current-year

[@emiplegiaqmnpm/hic-quibusdam-qui/is-data-property-in]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-data-property-in

[@emiplegiaqmnpm/hic-quibusdam-qui/is-data-property]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-data-property

[@emiplegiaqmnpm/hic-quibusdam-qui/is-dataview]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-dataview

[@emiplegiaqmnpm/hic-quibusdam-qui/is-digit-string]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-digit-string

[@emiplegiaqmnpm/hic-quibusdam-qui/is-domain-name]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-domain-name

[@emiplegiaqmnpm/hic-quibusdam-qui/is-duration-string]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-duration-string

[@emiplegiaqmnpm/hic-quibusdam-qui/is-email-address]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-email-address

[@emiplegiaqmnpm/hic-quibusdam-qui/is-empty-collection]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-empty-collection

[@emiplegiaqmnpm/hic-quibusdam-qui/is-empty-object]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-empty-object

[@emiplegiaqmnpm/hic-quibusdam-qui/is-empty-string]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-empty-string

[@emiplegiaqmnpm/hic-quibusdam-qui/is-enumerable-property-in]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-enumerable-property-in

[@emiplegiaqmnpm/hic-quibusdam-qui/is-enumerable-property]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-enumerable-property

[@emiplegiaqmnpm/hic-quibusdam-qui/is-even]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-even

[@emiplegiaqmnpm/hic-quibusdam-qui/is-falsy]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-falsy

[@emiplegiaqmnpm/hic-quibusdam-qui/is-finite]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-finite

[@emiplegiaqmnpm/hic-quibusdam-qui/is-generator-object-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-generator-object-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-generator-object]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-generator-object

[@emiplegiaqmnpm/hic-quibusdam-qui/is-gzip-buffer]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-gzip-buffer

[@emiplegiaqmnpm/hic-quibusdam-qui/is-hex-string]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-hex-string

[@emiplegiaqmnpm/hic-quibusdam-qui/is-infinite]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-infinite

[@emiplegiaqmnpm/hic-quibusdam-qui/is-inherited-property]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-inherited-property

[@emiplegiaqmnpm/hic-quibusdam-qui/is-iterable-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-iterable-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-iterator-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-iterator-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-json]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-json

[@emiplegiaqmnpm/hic-quibusdam-qui/is-kebabcase]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-kebabcase

[@emiplegiaqmnpm/hic-quibusdam-qui/is-leap-year]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-leap-year

[@emiplegiaqmnpm/hic-quibusdam-qui/is-localhost]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-localhost

[@emiplegiaqmnpm/hic-quibusdam-qui/is-lowercase]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-lowercase

[@emiplegiaqmnpm/hic-quibusdam-qui/is-method-in]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-method-in

[@emiplegiaqmnpm/hic-quibusdam-qui/is-method]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-method

[@emiplegiaqmnpm/hic-quibusdam-qui/is-multi-slice]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-multi-slice

[@emiplegiaqmnpm/hic-quibusdam-qui/is-named-typed-tuple-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-named-typed-tuple-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-native-function]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-native-function

[@emiplegiaqmnpm/hic-quibusdam-qui/is-negative-zero]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-negative-zero

[@emiplegiaqmnpm/hic-quibusdam-qui/is-node-builtin]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-node-builtin

[@emiplegiaqmnpm/hic-quibusdam-qui/is-node-duplex-stream-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-node-duplex-stream-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-node-readable-stream-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-node-readable-stream-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-node-repl]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-node-repl

[@emiplegiaqmnpm/hic-quibusdam-qui/is-node-stream-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-node-stream-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-node-transform-stream-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-node-transform-stream-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-node-writable-stream-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-node-writable-stream-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-nonconfigurable-property-in]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-nonconfigurable-property-in

[@emiplegiaqmnpm/hic-quibusdam-qui/is-nonconfigurable-property]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-nonconfigurable-property

[@emiplegiaqmnpm/hic-quibusdam-qui/is-nonenumerable-property-in]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-nonenumerable-property-in

[@emiplegiaqmnpm/hic-quibusdam-qui/is-nonenumerable-property]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-nonenumerable-property

[@emiplegiaqmnpm/hic-quibusdam-qui/is-nonnegative-finite]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-nonnegative-finite

[@emiplegiaqmnpm/hic-quibusdam-qui/is-object-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-object-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-odd]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-odd

[@emiplegiaqmnpm/hic-quibusdam-qui/is-pascalcase]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-pascalcase

[@emiplegiaqmnpm/hic-quibusdam-qui/is-plain-object]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-plain-object

[@emiplegiaqmnpm/hic-quibusdam-qui/is-positive-zero]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-positive-zero

[@emiplegiaqmnpm/hic-quibusdam-qui/is-prime]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-prime

[@emiplegiaqmnpm/hic-quibusdam-qui/is-primitive]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-primitive

[@emiplegiaqmnpm/hic-quibusdam-qui/is-prng-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-prng-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-probability]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-probability

[@emiplegiaqmnpm/hic-quibusdam-qui/is-property-key]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-property-key

[@emiplegiaqmnpm/hic-quibusdam-qui/is-prototype-of]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-prototype-of

[@emiplegiaqmnpm/hic-quibusdam-qui/is-read-only-property-in]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-read-only-property-in

[@emiplegiaqmnpm/hic-quibusdam-qui/is-read-only-property]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-read-only-property

[@emiplegiaqmnpm/hic-quibusdam-qui/is-read-write-property-in]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-read-write-property-in

[@emiplegiaqmnpm/hic-quibusdam-qui/is-read-write-property]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-read-write-property

[@emiplegiaqmnpm/hic-quibusdam-qui/is-readable-property-in]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-readable-property-in

[@emiplegiaqmnpm/hic-quibusdam-qui/is-readable-property]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-readable-property

[@emiplegiaqmnpm/hic-quibusdam-qui/is-regexp-string]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-regexp-string

[@emiplegiaqmnpm/hic-quibusdam-qui/is-relative-path]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-relative-path

[@emiplegiaqmnpm/hic-quibusdam-qui/is-relative-uri]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-relative-uri

[@emiplegiaqmnpm/hic-quibusdam-qui/is-same-complex128]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-same-complex128

[@emiplegiaqmnpm/hic-quibusdam-qui/is-same-complex64]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-same-complex64

[@emiplegiaqmnpm/hic-quibusdam-qui/is-same-native-class]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-same-native-class

[@emiplegiaqmnpm/hic-quibusdam-qui/is-same-type]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-same-type

[@emiplegiaqmnpm/hic-quibusdam-qui/is-same-value-zero]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-same-value-zero

[@emiplegiaqmnpm/hic-quibusdam-qui/is-same-value]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-same-value

[@emiplegiaqmnpm/hic-quibusdam-qui/is-semver]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-semver

[@emiplegiaqmnpm/hic-quibusdam-qui/is-slice]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-slice

[@emiplegiaqmnpm/hic-quibusdam-qui/is-snakecase]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-snakecase

[@emiplegiaqmnpm/hic-quibusdam-qui/is-startcase]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-startcase

[@emiplegiaqmnpm/hic-quibusdam-qui/is-strict-equal]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-strict-equal

[@emiplegiaqmnpm/hic-quibusdam-qui/is-truthy]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-truthy

[@emiplegiaqmnpm/hic-quibusdam-qui/is-unc-path]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-unc-path

[@emiplegiaqmnpm/hic-quibusdam-qui/is-undefined-or-null]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-undefined-or-null

[@emiplegiaqmnpm/hic-quibusdam-qui/is-uppercase]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-uppercase

[@emiplegiaqmnpm/hic-quibusdam-qui/is-uri]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-uri

[@emiplegiaqmnpm/hic-quibusdam-qui/is-whitespace]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-whitespace

[@emiplegiaqmnpm/hic-quibusdam-qui/is-writable-property-in]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-writable-property-in

[@emiplegiaqmnpm/hic-quibusdam-qui/is-writable-property]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-writable-property

[@emiplegiaqmnpm/hic-quibusdam-qui/is-write-only-property-in]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-write-only-property-in

[@emiplegiaqmnpm/hic-quibusdam-qui/is-write-only-property]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-write-only-property

[@emiplegiaqmnpm/hic-quibusdam-qui/tools]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/tools

[@emiplegiaqmnpm/hic-quibusdam-qui/has-arraybuffer-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-arraybuffer-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-arrow-function-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-arrow-function-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-async-await-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-async-await-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-async-iterator-symbol-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-async-iterator-symbol-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-bigint-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-bigint-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-bigint64array-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-bigint64array-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-biguint64array-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-biguint64array-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-class-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-class-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-dataview-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-dataview-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-define-properties-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-define-properties-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-define-property-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-define-property-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-float32array-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-float32array-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-float64array-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-float64array-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-function-name-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-function-name-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-generator-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-generator-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-globalthis-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-globalthis-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-int16array-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-int16array-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-int32array-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-int32array-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-int8array-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-int8array-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-iterator-symbol-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-iterator-symbol-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-map-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-map-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-node-buffer-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-node-buffer-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-proxy-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-proxy-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-set-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-set-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-sharedarraybuffer-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-sharedarraybuffer-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-symbol-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-symbol-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-tostringtag-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-tostringtag-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-uint16array-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-uint16array-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-uint32array-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-uint32array-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-uint8array-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-uint8array-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-uint8clampedarray-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-uint8clampedarray-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-wasm-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-wasm-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-weakmap-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-weakmap-support

[@emiplegiaqmnpm/hic-quibusdam-qui/has-weakset-support]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/has-weakset-support

[@emiplegiaqmnpm/hic-quibusdam-qui/is-big-endian]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-big-endian

[@emiplegiaqmnpm/hic-quibusdam-qui/is-browser]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-browser

[@emiplegiaqmnpm/hic-quibusdam-qui/is-darwin]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-darwin

[@emiplegiaqmnpm/hic-quibusdam-qui/is-docker]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-docker

[@emiplegiaqmnpm/hic-quibusdam-qui/is-electron-main]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-electron-main

[@emiplegiaqmnpm/hic-quibusdam-qui/is-electron-renderer]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-electron-renderer

[@emiplegiaqmnpm/hic-quibusdam-qui/is-electron]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-electron

[@emiplegiaqmnpm/hic-quibusdam-qui/is-little-endian]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-little-endian

[@emiplegiaqmnpm/hic-quibusdam-qui/is-mobile]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-mobile

[@emiplegiaqmnpm/hic-quibusdam-qui/is-node]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-node

[@emiplegiaqmnpm/hic-quibusdam-qui/is-touch-device]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-touch-device

[@emiplegiaqmnpm/hic-quibusdam-qui/is-web-worker]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-web-worker

[@emiplegiaqmnpm/hic-quibusdam-qui/is-windows]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-windows

[@emiplegiaqmnpm/hic-quibusdam-qui/is-error]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-error

[@emiplegiaqmnpm/hic-quibusdam-qui/is-eval-error]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-eval-error

[@emiplegiaqmnpm/hic-quibusdam-qui/is-range-error]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-range-error

[@emiplegiaqmnpm/hic-quibusdam-qui/is-reference-error]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-reference-error

[@emiplegiaqmnpm/hic-quibusdam-qui/is-syntax-error]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-syntax-error

[@emiplegiaqmnpm/hic-quibusdam-qui/is-type-error]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-type-error

[@emiplegiaqmnpm/hic-quibusdam-qui/is-uri-error]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-uri-error

[@emiplegiaqmnpm/hic-quibusdam-qui/is-accessor-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-accessor-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-array-length]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-array-length

[@emiplegiaqmnpm/hic-quibusdam-qui/is-array-like-object]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-array-like-object

[@emiplegiaqmnpm/hic-quibusdam-qui/is-array-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-array-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-arraybuffer-view]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-arraybuffer-view

[@emiplegiaqmnpm/hic-quibusdam-qui/is-arraybuffer]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-arraybuffer

[@emiplegiaqmnpm/hic-quibusdam-qui/is-between-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-between-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-bigint64array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-bigint64array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-biguint64array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-biguint64array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-circular-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-circular-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-empty-array-like-object]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-empty-array-like-object

[@emiplegiaqmnpm/hic-quibusdam-qui/is-empty-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-empty-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-falsy-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-falsy-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-finite-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-finite-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-numeric-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-numeric-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-plain-object-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-plain-object-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-probability-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-probability-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-same-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-same-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-same-complex128array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-same-complex128array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-same-complex64array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-same-complex64array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-same-float32array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-same-float32array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-same-float64array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-same-float64array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-sharedarraybuffer]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-sharedarraybuffer

[@emiplegiaqmnpm/hic-quibusdam-qui/is-truthy-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-truthy-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-typed-array-length]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-typed-array-length

[@emiplegiaqmnpm/hic-quibusdam-qui/is-typed-array-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-typed-array-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-typed-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-typed-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-unity-probability-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-unity-probability-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-complex-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-complex-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-complex-typed-array-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-complex-typed-array-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-complex-typed-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-complex-typed-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-complex]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-complex

[@emiplegiaqmnpm/hic-quibusdam-qui/is-complex128]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-complex128

[@emiplegiaqmnpm/hic-quibusdam-qui/is-complex128array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-complex128array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-complex64]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-complex64

[@emiplegiaqmnpm/hic-quibusdam-qui/is-complex64array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-complex64array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-centrosymmetric-matrix]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-centrosymmetric-matrix

[@emiplegiaqmnpm/hic-quibusdam-qui/is-complex128matrix-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-complex128matrix-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-complex128ndarray-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-complex128ndarray-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-complex128vector-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-complex128vector-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-complex64matrix-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-complex64matrix-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-complex64ndarray-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-complex64ndarray-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-complex64vector-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-complex64vector-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-float32matrix-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-float32matrix-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-float32ndarray-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-float32ndarray-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-float32vector-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-float32vector-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-float64matrix-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-float64matrix-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-float64ndarray-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-float64ndarray-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-float64vector-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-float64vector-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-matrix-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-matrix-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-ndarray-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-ndarray-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-nonsymmetric-matrix]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-nonsymmetric-matrix

[@emiplegiaqmnpm/hic-quibusdam-qui/is-persymmetric-matrix]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-persymmetric-matrix

[@emiplegiaqmnpm/hic-quibusdam-qui/is-skew-centrosymmetric-matrix]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-skew-centrosymmetric-matrix

[@emiplegiaqmnpm/hic-quibusdam-qui/is-skew-persymmetric-matrix]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-skew-persymmetric-matrix

[@emiplegiaqmnpm/hic-quibusdam-qui/is-skew-symmetric-matrix]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-skew-symmetric-matrix

[@emiplegiaqmnpm/hic-quibusdam-qui/is-square-matrix]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-square-matrix

[@emiplegiaqmnpm/hic-quibusdam-qui/is-symmetric-matrix]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-symmetric-matrix

[@emiplegiaqmnpm/hic-quibusdam-qui/is-vector-like]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-vector-like

[@emiplegiaqmnpm/hic-quibusdam-qui/is-float32array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-float32array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-float64array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-float64array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-int16array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-int16array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-int32array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-int32array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-int8array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-int8array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-uint16array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-uint16array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-uint32array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-uint32array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-uint8array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-uint8array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-uint8clampedarray]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-uint8clampedarray

[@emiplegiaqmnpm/hic-quibusdam-qui/is-cube-number]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-cube-number

[@emiplegiaqmnpm/hic-quibusdam-qui/is-integer-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-integer-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-integer]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-integer

[@emiplegiaqmnpm/hic-quibusdam-qui/is-negative-integer-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-negative-integer-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-negative-integer]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-negative-integer

[@emiplegiaqmnpm/hic-quibusdam-qui/is-negative-number-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-negative-number-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-negative-number]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-negative-number

[@emiplegiaqmnpm/hic-quibusdam-qui/is-nonnegative-integer-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-nonnegative-integer-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-nonnegative-integer]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-nonnegative-integer

[@emiplegiaqmnpm/hic-quibusdam-qui/is-nonnegative-number-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-nonnegative-number-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-nonnegative-number]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-nonnegative-number

[@emiplegiaqmnpm/hic-quibusdam-qui/is-nonpositive-integer-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-nonpositive-integer-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-nonpositive-integer]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-nonpositive-integer

[@emiplegiaqmnpm/hic-quibusdam-qui/is-nonpositive-number-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-nonpositive-number-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-nonpositive-number]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-nonpositive-number

[@emiplegiaqmnpm/hic-quibusdam-qui/is-positive-integer-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-positive-integer-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-positive-integer]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-positive-integer

[@emiplegiaqmnpm/hic-quibusdam-qui/is-positive-number-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-positive-number-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-positive-number]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-positive-number

[@emiplegiaqmnpm/hic-quibusdam-qui/is-safe-integer-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-safe-integer-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-safe-integer]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-safe-integer

[@emiplegiaqmnpm/hic-quibusdam-qui/is-square-number]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-square-number

[@emiplegiaqmnpm/hic-quibusdam-qui/is-square-triangular-number]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-square-triangular-number

[@emiplegiaqmnpm/hic-quibusdam-qui/is-triangular-number]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-triangular-number

[@emiplegiaqmnpm/hic-quibusdam-qui/is-array-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-array-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-boolean-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-boolean-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-date-object-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-date-object-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-function-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-function-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-nan-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-nan-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-null-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-null-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-number-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-number-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-object-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-object-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-string-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-string-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-symbol-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-symbol-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-array]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-array

[@emiplegiaqmnpm/hic-quibusdam-qui/is-boolean]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-boolean

[@emiplegiaqmnpm/hic-quibusdam-qui/is-date-object]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-date-object

[@emiplegiaqmnpm/hic-quibusdam-qui/is-function]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-function

[@emiplegiaqmnpm/hic-quibusdam-qui/is-nan]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-nan

[@emiplegiaqmnpm/hic-quibusdam-qui/is-null]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-null

[@emiplegiaqmnpm/hic-quibusdam-qui/is-number]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-number

[@emiplegiaqmnpm/hic-quibusdam-qui/is-object]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-object

[@emiplegiaqmnpm/hic-quibusdam-qui/is-regexp]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-regexp

[@emiplegiaqmnpm/hic-quibusdam-qui/is-string]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-string

[@emiplegiaqmnpm/hic-quibusdam-qui/is-symbol]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-symbol

[@emiplegiaqmnpm/hic-quibusdam-qui/is-undefined]: https://github.com/emiplegiaqmnpm/hic-quibusdam-qui/tree/main/is-undefined

<!-- </toc-links> -->

</section>

<!-- /.links -->
