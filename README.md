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

# Arrays

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Arrays.

<section class="installation">

## Installation

```bash
npm install @f1stnpm2/non-tempora-eius
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
var ns = require( '@f1stnpm2/non-tempora-eius' );
```

#### ns

Arrays.

```javascript
var o = ns;
// returns {...}
```

The namespace exports the following array constructors:

<!-- <toc pattern="+(int*|float*|uint*|*buffer)"> -->

<div class="namespace-toc">

-   <span class="signature">[`ArrayBuffer( size )`][@f1stnpm2/non-tempora-eius/buffer]</span><span class="delimiter">: </span><span class="description">constructor which returns an object used to represent a generic, fixed-length raw binary data buffer.</span>
-   <span class="signature">[`Float32Array()`][@f1stnpm2/non-tempora-eius/float32]</span><span class="delimiter">: </span><span class="description">typed array constructor which returns a typed array representing an array of single-precision floating-point numbers in the platform byte order.</span>
-   <span class="signature">[`Float64Array()`][@f1stnpm2/non-tempora-eius/float64]</span><span class="delimiter">: </span><span class="description">typed array constructor which returns a typed array representing an array of double-precision floating-point numbers in the platform byte order.</span>
-   <span class="signature">[`Int16Array()`][@f1stnpm2/non-tempora-eius/int16]</span><span class="delimiter">: </span><span class="description">typed array constructor which returns a typed array representing an array of twos-complement 16-bit signed integers in the platform byte order.</span>
-   <span class="signature">[`Int32Array()`][@f1stnpm2/non-tempora-eius/int32]</span><span class="delimiter">: </span><span class="description">typed array constructor which returns a typed array representing an array of twos-complement 32-bit signed integers in the platform byte order.</span>
-   <span class="signature">[`Int8Array()`][@f1stnpm2/non-tempora-eius/int8]</span><span class="delimiter">: </span><span class="description">typed array constructor which returns a typed array representing an array of twos-complement 8-bit signed integers in the platform byte order.</span>
-   <span class="signature">[`SharedArrayBuffer( size )`][@f1stnpm2/non-tempora-eius/shared-buffer]</span><span class="delimiter">: </span><span class="description">constructor returning an object used to represent a generic, fixed-length raw binary data buffer which can be used to create views of shared memory.</span>
-   <span class="signature">[`Uint16Array()`][@f1stnpm2/non-tempora-eius/uint16]</span><span class="delimiter">: </span><span class="description">typed array constructor which returns a typed array representing an array of 16-bit unsigned integers in the platform byte order.</span>
-   <span class="signature">[`Uint32Array()`][@f1stnpm2/non-tempora-eius/uint32]</span><span class="delimiter">: </span><span class="description">typed array constructor which returns a typed array representing an array of 32-bit unsigned integers in the platform byte order.</span>
-   <span class="signature">[`Uint8Array()`][@f1stnpm2/non-tempora-eius/uint8]</span><span class="delimiter">: </span><span class="description">typed array constructor which returns a typed array representing an array of 8-bit unsigned integers in the platform byte order.</span>
-   <span class="signature">[`Uint8ClampedArray()`][@f1stnpm2/non-tempora-eius/uint8c]</span><span class="delimiter">: </span><span class="description">typed array constructor which returns a typed array representing an array of 8-bit unsigned integers in the platform byte order clamped to 0-255.</span>

</div>

<!-- </toc> -->

```javascript
var arr = new ns.Int32Array( 5 );
// returns <Int32Array>[ 0, 0, 0, 0, 0 ]
```

Alternatively, use the `typedarray` function to create a typed array of a given data type:

<!-- <toc pattern="typed"> -->

<div class="namespace-toc">

-   <span class="signature">[`typedarray()`][@f1stnpm2/non-tempora-eius/typed]</span><span class="delimiter">: </span><span class="description">create a typed array.</span>

</div>

<!-- </toc> -->

```javascript
var arr1 = ns.typedarray( 5 );
// returns <Float64Array>[ 0.0, 0.0, 0.0, 0.0, 0.0 ]

var arr2 = ns.typedarray( 5, 'uint8' );
// returns <Uint8Array>[ 0, 0, 0, 0, 0 ]
```

The namespace contains functions to create arrays pre-filled with spaced values:

<!-- <toc pattern="*space"> -->

<div class="namespace-toc">

-   <span class="signature">[`datespace( start, stop[, length][, opts] )`][@f1stnpm2/non-tempora-eius/datespace]</span><span class="delimiter">: </span><span class="description">generate an array of linearly spaced dates.</span>
-   <span class="signature">[`incrspace( start, stop[, increment] )`][@f1stnpm2/non-tempora-eius/incrspace]</span><span class="delimiter">: </span><span class="description">generate a linearly spaced numeric array using a provided increment.</span>
-   <span class="signature">[`linspace( start, stop, length[, options] )`][@f1stnpm2/non-tempora-eius/linspace]</span><span class="delimiter">: </span><span class="description">generate a linearly spaced array over a specified interval.</span>
-   <span class="signature">[`logspace( a, b[, length] )`][@f1stnpm2/non-tempora-eius/logspace]</span><span class="delimiter">: </span><span class="description">generate a logarithmically spaced numeric array.</span>

</div>

<!-- </toc> -->

You can use the following functions to retrieve a list of available data types:

<!-- <toc pattern="*dtypes"> -->

<div class="namespace-toc">

-   <span class="signature">[`dtypes( [kind] )`][@f1stnpm2/non-tempora-eius/dtypes]</span><span class="delimiter">: </span><span class="description">list of array data types.</span>
-   <span class="signature">[`complexarrayDataTypes()`][@f1stnpm2/non-tempora-eius/typed-complex-dtypes]</span><span class="delimiter">: </span><span class="description">list of complex typed array data types.</span>
-   <span class="signature">[`typedarrayDataTypes()`][@f1stnpm2/non-tempora-eius/typed-dtypes]</span><span class="delimiter">: </span><span class="description">list of typed array data types.</span>
-   <span class="signature">[`floatarrayDataTypes()`][@f1stnpm2/non-tempora-eius/typed-float-dtypes]</span><span class="delimiter">: </span><span class="description">list of typed array floating-point data types.</span>
-   <span class="signature">[`intarrayDataTypes()`][@f1stnpm2/non-tempora-eius/typed-integer-dtypes]</span><span class="delimiter">: </span><span class="description">list of typed array integer data types.</span>
-   <span class="signature">[`realarrayDataTypes()`][@f1stnpm2/non-tempora-eius/typed-real-dtypes]</span><span class="delimiter">: </span><span class="description">list of typed array real-valued data types.</span>
-   <span class="signature">[`realarrayFloatDataTypes()`][@f1stnpm2/non-tempora-eius/typed-real-float-dtypes]</span><span class="delimiter">: </span><span class="description">list of typed array real-valued floating-point data types.</span>
-   <span class="signature">[`intarraySignedDataTypes()`][@f1stnpm2/non-tempora-eius/typed-signed-integer-dtypes]</span><span class="delimiter">: </span><span class="description">list of typed array signed integer data types.</span>
-   <span class="signature">[`intarrayUnsignedDataTypes()`][@f1stnpm2/non-tempora-eius/typed-unsigned-integer-dtypes]</span><span class="delimiter">: </span><span class="description">list of typed array unsigned integer data types.</span>

</div>

<!-- </toc> -->

Furthermore, the namespace contains utility functions to retrieve a given constructor:

<!-- <toc keywords="+constructors,+constructor"> -->

<div class="namespace-toc">

-   <span class="signature">[`ctors( dtype )`][@f1stnpm2/non-tempora-eius/ctors]</span><span class="delimiter">: </span><span class="description">array constructors.</span>
-   <span class="signature">[`ArrayIndex( x[, options] )`][@f1stnpm2/non-tempora-eius/index]</span><span class="delimiter">: </span><span class="description">array index constructor.</span>
-   <span class="signature">[`complexarrayCtors( dtype )`][@f1stnpm2/non-tempora-eius/typed-complex-ctors]</span><span class="delimiter">: </span><span class="description">complex typed array constructors.</span>
-   <span class="signature">[`typedarrayCtors( dtype )`][@f1stnpm2/non-tempora-eius/typed-ctors]</span><span class="delimiter">: </span><span class="description">typed array constructors.</span>
-   <span class="signature">[`floatarrayCtors( dtype )`][@f1stnpm2/non-tempora-eius/typed-float-ctors]</span><span class="delimiter">: </span><span class="description">floating-point typed array constructors.</span>
-   <span class="signature">[`intarrayCtors( dtype )`][@f1stnpm2/non-tempora-eius/typed-integer-ctors]</span><span class="delimiter">: </span><span class="description">integer-valued typed array constructors.</span>
-   <span class="signature">[`realarrayCtors( dtype )`][@f1stnpm2/non-tempora-eius/typed-real-ctors]</span><span class="delimiter">: </span><span class="description">typed array constructors.</span>
-   <span class="signature">[`realarrayFloatCtors( dtype )`][@f1stnpm2/non-tempora-eius/typed-real-float-ctors]</span><span class="delimiter">: </span><span class="description">real-valued floating-point typed array constructors.</span>
-   <span class="signature">[`intarraySignedCtors( dtype )`][@f1stnpm2/non-tempora-eius/typed-signed-integer-ctors]</span><span class="delimiter">: </span><span class="description">signed integer typed array constructors.</span>
-   <span class="signature">[`intarrayUnsignedCtors( dtype )`][@f1stnpm2/non-tempora-eius/typed-unsigned-integer-ctors]</span><span class="delimiter">: </span><span class="description">unsigned integer typed array constructors.</span>

</div>

<!-- </toc> -->

```javascript
var ctor = ns.typedarrayCtors( 'float64' );
// returns <Function>

ctor = ns.typedarrayCtors( 'int' );
// returns null
```

Lastly, the namespace contains various other functions for dealing with arrays, including functions to convert arrays from one data type to another or to serialize them as JSON and vice versa.

<!-- <toc ignore="+(int*|float*|uint*|*buffer)" ignore="typed" ignore="*dtypes" keywords="-constructors,-constructor"> -->

<div class="namespace-toc">

-   <span class="signature">[`base`][@f1stnpm2/non-tempora-eius/base]</span><span class="delimiter">: </span><span class="description">base (i.e., lower-level) array utilities.</span>
-   <span class="signature">[`cartesianPower( x, n )`][@f1stnpm2/non-tempora-eius/cartesian-power]</span><span class="delimiter">: </span><span class="description">return the Cartesian power.</span>
-   <span class="signature">[`cartesianProduct( x1, x2 )`][@f1stnpm2/non-tempora-eius/cartesian-product]</span><span class="delimiter">: </span><span class="description">return the Cartesian product.</span>
-   <span class="signature">[`cartesianSquare( x )`][@f1stnpm2/non-tempora-eius/cartesian-square]</span><span class="delimiter">: </span><span class="description">return the Cartesian square.</span>
-   <span class="signature">[`Complex128Array()`][@f1stnpm2/non-tempora-eius/complex128]</span><span class="delimiter">: </span><span class="description">128-bit complex number array.</span>
-   <span class="signature">[`Complex64Array()`][@f1stnpm2/non-tempora-eius/complex64]</span><span class="delimiter">: </span><span class="description">64-bit complex number array.</span>
-   <span class="signature">[`convertSame( x, y )`][@f1stnpm2/non-tempora-eius/convert-same]</span><span class="delimiter">: </span><span class="description">convert an array to the same data type as a second input array.</span>
-   <span class="signature">[`convert( arr, dtype )`][@f1stnpm2/non-tempora-eius/convert]</span><span class="delimiter">: </span><span class="description">convert an array to an array of a different data type.</span>
-   <span class="signature">[`DataView( buffer[, byteOffset[, byteLength]] )`][@f1stnpm2/non-tempora-eius/dataview]</span><span class="delimiter">: </span><span class="description">constructor which returns a data view representing a provided array buffer.</span>
-   <span class="signature">[`defaults()`][@f1stnpm2/non-tempora-eius/defaults]</span><span class="delimiter">: </span><span class="description">default array settings.</span>
-   <span class="signature">[`dtype( array )`][@f1stnpm2/non-tempora-eius/dtype]</span><span class="delimiter">: </span><span class="description">return the data type of an array.</span>
-   <span class="signature">[`emptyLike( x[, dtype] )`][@f1stnpm2/non-tempora-eius/empty-like]</span><span class="delimiter">: </span><span class="description">create an uninitialized array having the same length and data type as a provided array.</span>
-   <span class="signature">[`empty( length[, dtype] )`][@f1stnpm2/non-tempora-eius/empty]</span><span class="delimiter">: </span><span class="description">create an uninitialized array having a specified length.</span>
-   <span class="signature">[`filledBy()`][@f1stnpm2/non-tempora-eius/filled-by]</span><span class="delimiter">: </span><span class="description">create a filled array according to a provided callback function.</span>
-   <span class="signature">[`filled()`][@f1stnpm2/non-tempora-eius/filled]</span><span class="delimiter">: </span><span class="description">create a filled array.</span>
-   <span class="signature">[`iterator2array( iterator[, out][, mapFcn[, thisArg]] )`][@f1stnpm2/non-tempora-eius/from-iterator]</span><span class="delimiter">: </span><span class="description">create (or fill) an array from an iterator.</span>
-   <span class="signature">[`scalar2array( value[, dtype] )`][@f1stnpm2/non-tempora-eius/from-scalar]</span><span class="delimiter">: </span><span class="description">create a single-element array containing a provided scalar value.</span>
-   <span class="signature">[`fullLike( x, value[, dtype] )`][@f1stnpm2/non-tempora-eius/full-like]</span><span class="delimiter">: </span><span class="description">create a filled array having the same length and data type as a provided array.</span>
-   <span class="signature">[`full( length, value[, dtype] )`][@f1stnpm2/non-tempora-eius/full]</span><span class="delimiter">: </span><span class="description">create a filled array having a specified length.</span>
-   <span class="signature">[`minDataType( value )`][@f1stnpm2/non-tempora-eius/min-dtype]</span><span class="delimiter">: </span><span class="description">determine the minimum array data type of the closest "kind" necessary for storing a provided scalar value.</span>
-   <span class="signature">[`mostlySafeCasts( [dtype] )`][@f1stnpm2/non-tempora-eius/mostly-safe-casts]</span><span class="delimiter">: </span><span class="description">return a list of array data types to which a provided array data type can be safely cast and, for floating-point data types, can be downcast.</span>
-   <span class="signature">[`mskfilter( x, mask )`][@f1stnpm2/non-tempora-eius/mskfilter]</span><span class="delimiter">: </span><span class="description">apply a mask to a provided input array.</span>
-   <span class="signature">[`mskreject( x, mask )`][@f1stnpm2/non-tempora-eius/mskreject]</span><span class="delimiter">: </span><span class="description">apply a mask to a provided input array.</span>
-   <span class="signature">[`nansLike( x[, dtype] )`][@f1stnpm2/non-tempora-eius/nans-like]</span><span class="delimiter">: </span><span class="description">create an array filled with NaNs and having the same length and data type as a provided array.</span>
-   <span class="signature">[`nans( length[, dtype] )`][@f1stnpm2/non-tempora-eius/nans]</span><span class="delimiter">: </span><span class="description">create an array filled with NaNs and having a specified length.</span>
-   <span class="signature">[`nextDataType( [dtype] )`][@f1stnpm2/non-tempora-eius/next-dtype]</span><span class="delimiter">: </span><span class="description">return the next larger array data type of the same kind.</span>
-   <span class="signature">[`oneToLike( x[, dtype] )`][@f1stnpm2/non-tempora-eius/one-to-like]</span><span class="delimiter">: </span><span class="description">generate a linearly spaced numeric array whose elements increment by `1` starting from one and having the same length and data type as a provided input array.</span>
-   <span class="signature">[`oneTo( n[, dtype] )`][@f1stnpm2/non-tempora-eius/one-to]</span><span class="delimiter">: </span><span class="description">generate a linearly spaced numeric array whose elements increment by `1` starting from one.</span>
-   <span class="signature">[`onesLike( x[, dtype] )`][@f1stnpm2/non-tempora-eius/ones-like]</span><span class="delimiter">: </span><span class="description">create an array filled with ones and having the same length and data type as a provided array.</span>
-   <span class="signature">[`ones( length[, dtype] )`][@f1stnpm2/non-tempora-eius/ones]</span><span class="delimiter">: </span><span class="description">create an array filled with ones and having a specified length.</span>
-   <span class="signature">[`typedarraypool()`][@f1stnpm2/non-tempora-eius/pool]</span><span class="delimiter">: </span><span class="description">allocate typed arrays from a typed array memory pool.</span>
-   <span class="signature">[`promotionRules( [dtype1, dtype2] )`][@f1stnpm2/non-tempora-eius/promotion-rules]</span><span class="delimiter">: </span><span class="description">return the array data type with the smallest size and closest "kind" to which array data types can be **safely** cast.</span>
-   <span class="signature">[`typedarrayReviver( key, value )`][@f1stnpm2/non-tempora-eius/reviver]</span><span class="delimiter">: </span><span class="description">revive a JSON-serialized typed array.</span>
-   <span class="signature">[`safeCasts( [dtype] )`][@f1stnpm2/non-tempora-eius/safe-casts]</span><span class="delimiter">: </span><span class="description">return a list of array data types to which a provided array data type can be safely cast.</span>
-   <span class="signature">[`sameKindCasts( [dtype] )`][@f1stnpm2/non-tempora-eius/same-kind-casts]</span><span class="delimiter">: </span><span class="description">return a list of array data types to which a provided array data type can be safely cast or cast within the same "kind".</span>
-   <span class="signature">[`shape( arr )`][@f1stnpm2/non-tempora-eius/shape]</span><span class="delimiter">: </span><span class="description">determine (nested) array dimensions.</span>
-   <span class="signature">[`slice( x[, start[, end]] )`][@f1stnpm2/non-tempora-eius/slice]</span><span class="delimiter">: </span><span class="description">return a shallow copy of a portion of an array.</span>
-   <span class="signature">[`take( x, indices[, options] )`][@f1stnpm2/non-tempora-eius/take]</span><span class="delimiter">: </span><span class="description">take elements from an array.</span>
-   <span class="signature">[`circarray2iterator( src[, options][, mapFcn[, thisArg]] )`][@f1stnpm2/non-tempora-eius/to-circular-iterator]</span><span class="delimiter">: </span><span class="description">create an iterator which repeatedly iterates over the elements of an array-like object.</span>
-   <span class="signature">[`array2fancy( x[, options] )`][@f1stnpm2/non-tempora-eius/to-fancy]</span><span class="delimiter">: </span><span class="description">convert an array to an object supporting fancy indexing.</span>
-   <span class="signature">[`array2iteratorRight( src[, mapFcn[, thisArg]] )`][@f1stnpm2/non-tempora-eius/to-iterator-right]</span><span class="delimiter">: </span><span class="description">create an iterator from an array-like object, iterating from right to left.</span>
-   <span class="signature">[`array2iterator( src[, mapFcn[, thisArg]] )`][@f1stnpm2/non-tempora-eius/to-iterator]</span><span class="delimiter">: </span><span class="description">create an iterator from an array-like object.</span>
-   <span class="signature">[`typedarray2json( typedarray )`][@f1stnpm2/non-tempora-eius/to-json]</span><span class="delimiter">: </span><span class="description">return a JSON representation of a typed array.</span>
-   <span class="signature">[`sparsearray2iteratorRight( src[, mapFcn[, thisArg]] )`][@f1stnpm2/non-tempora-eius/to-sparse-iterator-right]</span><span class="delimiter">: </span><span class="description">create an iterator from a sparse array-like object, iterating from right to left.</span>
-   <span class="signature">[`sparsearray2iterator( src[, mapFcn[, thisArg]] )`][@f1stnpm2/non-tempora-eius/to-sparse-iterator]</span><span class="delimiter">: </span><span class="description">create an iterator from a sparse array-like object.</span>
-   <span class="signature">[`stridedarray2iterator( N, src, stride, offset[, mapFcn[, thisArg]] )`][@f1stnpm2/non-tempora-eius/to-strided-iterator]</span><span class="delimiter">: </span><span class="description">create an iterator from a strided array-like object.</span>
-   <span class="signature">[`arrayview2iteratorRight( src[, begin[, end]][, mapFcn[, thisArg]] )`][@f1stnpm2/non-tempora-eius/to-view-iterator-right]</span><span class="delimiter">: </span><span class="description">create an iterator from an array-like object view, iterating from right to left.</span>
-   <span class="signature">[`arrayview2iterator( src[, begin[, end]][, mapFcn[, thisArg]] )`][@f1stnpm2/non-tempora-eius/to-view-iterator]</span><span class="delimiter">: </span><span class="description">create an iterator from an array-like object view.</span>
-   <span class="signature">[`complexarray()`][@f1stnpm2/non-tempora-eius/typed-complex]</span><span class="delimiter">: </span><span class="description">create a complex number typed array.</span>
-   <span class="signature">[`realarray()`][@f1stnpm2/non-tempora-eius/typed-real]</span><span class="delimiter">: </span><span class="description">create a typed array.</span>
-   <span class="signature">[`zeroToLike( x[, dtype] )`][@f1stnpm2/non-tempora-eius/zero-to-like]</span><span class="delimiter">: </span><span class="description">generate a linearly spaced numeric array whose elements increment by `1` starting from zero and having the same length and data type as a provided input array.</span>
-   <span class="signature">[`zeroTo( n[, dtype] )`][@f1stnpm2/non-tempora-eius/zero-to]</span><span class="delimiter">: </span><span class="description">generate a linearly spaced numeric array whose elements increment by `1` starting from zero.</span>
-   <span class="signature">[`zerosLike( x[, dtype] )`][@f1stnpm2/non-tempora-eius/zeros-like]</span><span class="delimiter">: </span><span class="description">create a zero-filled array having the same length and data type as a provided array.</span>
-   <span class="signature">[`zeros( length[, dtype] )`][@f1stnpm2/non-tempora-eius/zeros]</span><span class="delimiter">: </span><span class="description">create a zero-filled array having a specified length.</span>

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
var ns = require( '@f1stnpm2/non-tempora-eius' );

console.log( objectKeys( ns ) );
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

[npm-image]: http://img.shields.io/npm/v/@f1stnpm2/non-tempora-eius.svg
[npm-url]: https://npmjs.org/package/@f1stnpm2/non-tempora-eius

[test-image]: https://github.com/f1stnpm2/non-tempora-eius/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/f1stnpm2/non-tempora-eius/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/f1stnpm2/non-tempora-eius/main.svg
[coverage-url]: https://codecov.io/github/f1stnpm2/non-tempora-eius?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/f1stnpm2/non-tempora-eius.svg
[dependencies-url]: https://david-dm.org/f1stnpm2/non-tempora-eius/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/f1stnpm2/non-tempora-eius/tree/deno
[deno-readme]: https://github.com/f1stnpm2/non-tempora-eius/blob/deno/README.md
[umd-url]: https://github.com/f1stnpm2/non-tempora-eius/tree/umd
[umd-readme]: https://github.com/f1stnpm2/non-tempora-eius/blob/umd/README.md
[esm-url]: https://github.com/f1stnpm2/non-tempora-eius/tree/esm
[esm-readme]: https://github.com/f1stnpm2/non-tempora-eius/blob/esm/README.md
[branches-url]: https://github.com/f1stnpm2/non-tempora-eius/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/f1stnpm2/non-tempora-eius/main/LICENSE

<!-- <toc-links> -->

[@f1stnpm2/non-tempora-eius/base]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/base

[@f1stnpm2/non-tempora-eius/cartesian-power]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/cartesian-power

[@f1stnpm2/non-tempora-eius/cartesian-product]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/cartesian-product

[@f1stnpm2/non-tempora-eius/cartesian-square]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/cartesian-square

[@f1stnpm2/non-tempora-eius/complex128]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/complex128

[@f1stnpm2/non-tempora-eius/complex64]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/complex64

[@f1stnpm2/non-tempora-eius/convert-same]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/convert-same

[@f1stnpm2/non-tempora-eius/convert]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/convert

[@f1stnpm2/non-tempora-eius/dataview]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/dataview

[@f1stnpm2/non-tempora-eius/defaults]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/defaults

[@f1stnpm2/non-tempora-eius/dtype]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/dtype

[@f1stnpm2/non-tempora-eius/empty-like]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/empty-like

[@f1stnpm2/non-tempora-eius/empty]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/empty

[@f1stnpm2/non-tempora-eius/filled-by]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/filled-by

[@f1stnpm2/non-tempora-eius/filled]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/filled

[@f1stnpm2/non-tempora-eius/from-iterator]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/from-iterator

[@f1stnpm2/non-tempora-eius/from-scalar]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/from-scalar

[@f1stnpm2/non-tempora-eius/full-like]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/full-like

[@f1stnpm2/non-tempora-eius/full]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/full

[@f1stnpm2/non-tempora-eius/min-dtype]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/min-dtype

[@f1stnpm2/non-tempora-eius/mostly-safe-casts]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/mostly-safe-casts

[@f1stnpm2/non-tempora-eius/mskfilter]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/mskfilter

[@f1stnpm2/non-tempora-eius/mskreject]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/mskreject

[@f1stnpm2/non-tempora-eius/nans-like]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/nans-like

[@f1stnpm2/non-tempora-eius/nans]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/nans

[@f1stnpm2/non-tempora-eius/next-dtype]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/next-dtype

[@f1stnpm2/non-tempora-eius/one-to-like]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/one-to-like

[@f1stnpm2/non-tempora-eius/one-to]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/one-to

[@f1stnpm2/non-tempora-eius/ones-like]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/ones-like

[@f1stnpm2/non-tempora-eius/ones]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/ones

[@f1stnpm2/non-tempora-eius/pool]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/pool

[@f1stnpm2/non-tempora-eius/promotion-rules]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/promotion-rules

[@f1stnpm2/non-tempora-eius/reviver]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/reviver

[@f1stnpm2/non-tempora-eius/safe-casts]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/safe-casts

[@f1stnpm2/non-tempora-eius/same-kind-casts]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/same-kind-casts

[@f1stnpm2/non-tempora-eius/shape]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/shape

[@f1stnpm2/non-tempora-eius/slice]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/slice

[@f1stnpm2/non-tempora-eius/take]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/take

[@f1stnpm2/non-tempora-eius/to-circular-iterator]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/to-circular-iterator

[@f1stnpm2/non-tempora-eius/to-fancy]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/to-fancy

[@f1stnpm2/non-tempora-eius/to-iterator-right]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/to-iterator-right

[@f1stnpm2/non-tempora-eius/to-iterator]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/to-iterator

[@f1stnpm2/non-tempora-eius/to-json]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/to-json

[@f1stnpm2/non-tempora-eius/to-sparse-iterator-right]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/to-sparse-iterator-right

[@f1stnpm2/non-tempora-eius/to-sparse-iterator]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/to-sparse-iterator

[@f1stnpm2/non-tempora-eius/to-strided-iterator]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/to-strided-iterator

[@f1stnpm2/non-tempora-eius/to-view-iterator-right]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/to-view-iterator-right

[@f1stnpm2/non-tempora-eius/to-view-iterator]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/to-view-iterator

[@f1stnpm2/non-tempora-eius/typed-complex]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/typed-complex

[@f1stnpm2/non-tempora-eius/typed-real]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/typed-real

[@f1stnpm2/non-tempora-eius/zero-to-like]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/zero-to-like

[@f1stnpm2/non-tempora-eius/zero-to]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/zero-to

[@f1stnpm2/non-tempora-eius/zeros-like]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/zeros-like

[@f1stnpm2/non-tempora-eius/zeros]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/zeros

[@f1stnpm2/non-tempora-eius/ctors]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/ctors

[@f1stnpm2/non-tempora-eius/index]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/index

[@f1stnpm2/non-tempora-eius/typed-complex-ctors]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/typed-complex-ctors

[@f1stnpm2/non-tempora-eius/typed-ctors]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/typed-ctors

[@f1stnpm2/non-tempora-eius/typed-float-ctors]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/typed-float-ctors

[@f1stnpm2/non-tempora-eius/typed-integer-ctors]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/typed-integer-ctors

[@f1stnpm2/non-tempora-eius/typed-real-ctors]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/typed-real-ctors

[@f1stnpm2/non-tempora-eius/typed-real-float-ctors]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/typed-real-float-ctors

[@f1stnpm2/non-tempora-eius/typed-signed-integer-ctors]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/typed-signed-integer-ctors

[@f1stnpm2/non-tempora-eius/typed-unsigned-integer-ctors]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/typed-unsigned-integer-ctors

[@f1stnpm2/non-tempora-eius/dtypes]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/dtypes

[@f1stnpm2/non-tempora-eius/typed-complex-dtypes]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/typed-complex-dtypes

[@f1stnpm2/non-tempora-eius/typed-dtypes]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/typed-dtypes

[@f1stnpm2/non-tempora-eius/typed-float-dtypes]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/typed-float-dtypes

[@f1stnpm2/non-tempora-eius/typed-integer-dtypes]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/typed-integer-dtypes

[@f1stnpm2/non-tempora-eius/typed-real-dtypes]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/typed-real-dtypes

[@f1stnpm2/non-tempora-eius/typed-real-float-dtypes]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/typed-real-float-dtypes

[@f1stnpm2/non-tempora-eius/typed-signed-integer-dtypes]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/typed-signed-integer-dtypes

[@f1stnpm2/non-tempora-eius/typed-unsigned-integer-dtypes]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/typed-unsigned-integer-dtypes

[@f1stnpm2/non-tempora-eius/datespace]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/datespace

[@f1stnpm2/non-tempora-eius/incrspace]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/incrspace

[@f1stnpm2/non-tempora-eius/linspace]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/linspace

[@f1stnpm2/non-tempora-eius/logspace]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/logspace

[@f1stnpm2/non-tempora-eius/typed]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/typed

[@f1stnpm2/non-tempora-eius/buffer]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/buffer

[@f1stnpm2/non-tempora-eius/float32]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/float32

[@f1stnpm2/non-tempora-eius/float64]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/float64

[@f1stnpm2/non-tempora-eius/int16]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/int16

[@f1stnpm2/non-tempora-eius/int32]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/int32

[@f1stnpm2/non-tempora-eius/int8]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/int8

[@f1stnpm2/non-tempora-eius/shared-buffer]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/shared-buffer

[@f1stnpm2/non-tempora-eius/uint16]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/uint16

[@f1stnpm2/non-tempora-eius/uint32]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/uint32

[@f1stnpm2/non-tempora-eius/uint8]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/uint8

[@f1stnpm2/non-tempora-eius/uint8c]: https://github.com/f1stnpm2/non-tempora-eius/tree/main/uint8c

<!-- </toc-links> -->

</section>

<!-- /.links -->
