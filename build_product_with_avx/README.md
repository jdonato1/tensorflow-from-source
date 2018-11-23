# build_product

This is the second build product:

* no avx instructions
* no avx2 instructions
* no XLA

The CPU actually had avx instruction set but apparently tensorflow is not compiled with avx if
avx2 is not available.

