# Try Python
Learn Python for data science.

## Table of contents
- [Built in functions](#built-in-functions)
- [Operations](#operations)
- [Order of operations](#order-of-operations)
- [Type conversion](#type-conversion)

### Built in functions
- print

code
```python
print('Hello World!')
```
output
```
Hello World!
```

- type

code
```python
print(type(1))
print(type(1.23))
print(type('aof'))
```
output
```
<class 'int'>
<class 'float'>
<class 'str'>
```

- min/max

code
```python
print(min(1, 2, 3, 4, 5))
print(max(1, 2, 3, 4, 5))
```
output
```
1
5
```

### Operations

code
```python
print(1 + 1)
print(1 - 1)
print(2 * 3)
print(6 / 3)   # Return float
print(5 // 3)  # Floor division return int
print(8 % 3)
print(2 ** 3)  # 2 power of 3
```
output
```
2
0
6
2.0
1
2
8
```

### Order of operations
Python using **PEMDAS** ( **P**arentheses, **E**xponents, **M**ultiplication/**D**ivision, **A**ddition/**S**ubtraction) convention.

### Type conversion

code
```python
print(int(1.23))
print(float(1))
print(int('456') + 78)
```
output
```
1
1.0
534
```
