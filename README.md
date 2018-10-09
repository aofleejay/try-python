# Try Python
Learn Python for data science.

## Table of contents
- [Built in functions](#built-in-functions)
- [Operations](#operations)
- [Order of operations](#order-of-operations)
- [Type conversion](#type-conversion)
- [Function](#function)
  - [Lambda](#lambda)

### Built in functions
- print
```
>>> print('Hello World!')
Hello World!
```

- type
```
>>> type(1)
<type 'int'>
>>> type(1.23)
<type 'float'>
>>> type('aof')
<type 'str'>
```

- min/max
```
>>> min(1, 2, 3, 4, 5)
1
>>> max(1, 2, 3, 4, 5)
5
```

### Operations
```
>>> 1 + 1
2
>>> 1 - 1
0
>>> 2 * 3
6
>>> 6 / 3
2.0
>>> 5 // 3
1
>>> 8 % 3
2
>>> 2 ** 3
8
```

### Order of operations
Python using **PEMDAS** ( **P**arentheses, **E**xponents, **M**ultiplication/**D**ivision, **A**ddition/**S**ubtraction) convention.

### Type conversion
```
>>> int(1.23)
1
>>> float(1)
1.0
>>> int('456') + 78
534
```

### Function
```
>>> def sum(a, b):
...     return a + b
...
>>> sum(1, 2)
3
```

#### Lambda
```
>>> sub = lambda a, b: a - b
>>> sub(5, 1)
4
```
