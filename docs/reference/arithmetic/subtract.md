# Function subtract

Subtract two values, `x - y`. Matrices are subtracted element wise.


## Syntax

```js
math.subtract(x, y)
```

### Parameters

Parameter | Type | Description
--------- | ---- | -----------
`x`       | Number &#124; BigNumber &#124; Boolean &#124; Complex &#124; Unit &#124; Array &#124; Matrix | Initial value
`y`       | Number &#124; BigNumber &#124; Boolean &#124; Complex &#124; Unit &#124; Array &#124; Matrix | Value to subtract from `x`

### Returns

Type | Description
---- | -----------
Number &#124; BigNumber &#124; Complex &#124; Unit &#124; Array &#124; Matrix | Subtraction of `x` and `y`, `x - y`


## Examples

```js
var math = mathjs();

math.subtract(5.3, 2);        // returns Number 3.3

var a = math.complex(2, 3);
var b = math.complex(4, 1);
math.subtract(a, b);          // returns Complex -2 + 2i

math.subtract([5, 7, 4], 4);  // returns Array [1, 3, 0]

var c = math.unit('2.1 km');
var d = math.unit('500m');
math.subtract(c, d);          // returns Unit 1.6 km
```


## See also

[add](add.md)