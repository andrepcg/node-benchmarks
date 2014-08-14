Node.JS
=======

String to Integer
-----------------
**winner**: `parseInt(a,10)`

    parseInt       x 40,305,021 ops/sec ±0.81% (95 runs sampled)
    parseInt(a,10) x 46,662,459 ops/sec ±1.48% (86 runs sampled)
    Math#floor     x 27,024,369 ops/sec ±0.98% (85 runs sampled)
    +a             x 21,231,481 ops/sec ±0.95% (96 runs sampled)
    ~~a            x 22,256,226 ops/sec ±0.99% (88 runs sampled)
    a | 0          x 23,038,167 ops/sec ±1.20% (86 runs sampled)
    a * 1          x 22,416,100 ops/sec ±0.81% (86 runs sampled)
    a / 1          x 21,630,212 ops/sec ±0.91% (95 runs sampled)
    a % Infinity   x 14,162,057 ops/sec ±0.58% (86 runs sampled)
    a >> 0         x 23,309,153 ops/sec ±1.12% (88 runs sampled)
    eval(a)        x 5,536,882  ops/sec ±0.56% (92 runs sampled)
    a ^ 0          x 23,444,139 ops/sec ±0.68% (90 runs sampled)

Rouding Numbers
---------------
**winner**: `Math#floor`

    Math#floor     x 91,614,523 ops/sec ±0.97% (96 runs sampled)
    parseInt       x 38,430,130 ops/sec ±0.91% (87 runs sampled)
    parseInt(a,10) x 45,367,806 ops/sec ±0.75% (96 runs sampled)
    ~~a            x 80,252,961 ops/sec ±1.84% (80 runs sampled)
    a | a          x 76,177,198 ops/sec ±0.29% (95 runs sampled)
    a | 0          x 74,004,737 ops/sec ±1.90% (78 runs sampled)
    a & a          x 74,687,728 ops/sec ±0.71% (93 runs sampled)
    a << 0         x 82,201,053 ops/sec ±1.27% (86 runs sampled)
    Int#toFixed    x 2,911,860  ops/sec ±0.69% (93 runs sampled)
    modulo         x 77,863,883 ops/sec ±1.04% (91 runs sampled)

Object Loop
-----------
**winner**: `for Object#keys.length`

    prop in Object         x 1,231,135 ops/sec ±0.25% (97 runs sampled)
    forEach Object#keys    x 1,962,596 ops/sec ±0.21% (100 runs sampled)
    for Object#keys.length x 3,286,807 ops/sec ±0.39% (97 runs sampled)

Array Filter
------------
**winner**: `lodash#filter`

    Array#filter      x 364,000 ops/sec ±1.86% (81 runs sampled)
    underscore#filter x 360,219 ops/sec ±1.70% (91 runs sampled)
    lodash#filter     x 920,773 ops/sec ±0.39% (99 runs sampled)

Removing Duplicates
-------------------
**winner**: `eliminateDuplicates`

    filterDuplicates    x 105,623 ops/sec ±0.69% (99 runs sampled)
    eliminateDuplicates x 200,035 ops/sec ±0.40% (92 runs sampled)
