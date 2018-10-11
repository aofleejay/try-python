# Try Python
Learn Python for data science.

# Table of contents
- [Built in functions](#built-in-functions)
- [Operations](#operations)
  - [Order of operations](#order-of-operations)
- [Type conversion](#type-conversion)
- [Function](#function)
  - [Lambda](#lambda)
- [Conditional](#conditional)
- [Lists](#lists)
- [Tuples](#tuples)
- [Loops](#loop)
  - [For loop](#for-loop)
    - [List comprehensions](#list-comprehensions)
  - [While loop](#while-loop)

# Built in functions
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
>>> type(True)
<type 'bool'>
```

- min/max
```
>>> min(1, 2, 3, 4, 5)
1
>>> max(1, 2, 3, 4, 5)
5
```

# Operations
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

## Order of operations
Python using **PEMDAS** ( **P**arentheses, **E**xponents, **M**ultiplication/**D**ivision, **A**ddition/**S**ubtraction) convention.

# Type conversion
```
>>> int(1.23)
1
>>> float(1)
1.0
>>> int('456') + 78
534
>>> bool(0)
False
```

# Function
```
>>> def sum(a, b):
...     return a + b
...
>>> sum(1, 2)
3
```

## Lambda
```
>>> sub = lambda a, b: a - b
>>> sub(5, 1)
4
```

# Conditional
```
>>> if x == 0:
...     print('Zero')
... elif x > 0:
...     print('Positive')
... else:
...     print('Negative')
```

# Lists
```
>>> animals = ['dog', 'cat', 'bird', 'fish', 'snake']
```
Access elements at the end
```
>>> animals[-1]
'snake'
```
Slicing from index 0 but not including index 3
```
>>> animals[0:3]
['dog', 'cat', 'bird']
>>> animals[:3]
['dog', 'cat', 'bird']
```
Slicing from index 2 to the end of the list
```
>>> animals[2:]
['bird', 'fish', 'snake']
```
Slicing last 3 elements
```
>>> animals[-3:]
['bird', 'fish', 'snake']
```
List functions
```
>>> len(animals)
5

>>> sorted(animals)
['bird', 'cat', 'dog', 'fish', 'snake']

>>> sum([1, 2, 3, 4, 5])
15

>>> animals.append('cow')
>>> animals
['dog', 'cat', 'bird', 'fish', 'snake', 'cow']

>>> animals.pop()
'cow'

>>> animals.index('fish')
3

>>> 'cat' in animals
True
```

# Tuples
```
>>> gender = ('male', 'female')
>>> gender
('male', 'female')
```
Tuple cannot be modified
```
>>> gender[0] = 'foo'
TypeError: 'tuple' object does not support item assignment
```
Variable assigment from tuple

```
>>> def getGender():
...     return ('male', 'female')
...
>>> maleLabel, femaleLabel = getGender()
>>> maleLabel
'male'
>>> femaleLabel
'female'
```

# Loops
## For loop
Loop over elements
```
>>> animals = ['dog', 'cat', 'bird', 'fish', 'snake']
>>> for animal in animals:
...     print(animal, end = ' ')
'dog' 'cat' 'bird' 'fish' 'snake'
```
Loop over index
```
>>> animals = ['dog', 'cat', 'bird', 'fish', 'snake']
>>> for i in range(len(animals)):
...     print(animals[i], end = ' ')
'dog' 'cat' 'bird' 'fish' 'snake'
```
Enumerate
```
>>> animals = ['dog', 'cat', 'bird', 'fish', 'snake']
>>> for i, animal in enumerate(animals):
...     print(i, animal, sep = ':', end = ', ')
0:'dog', 1:'cat', 2:'bird', 3:'fish', 4:'snake', 
```
### List comprehensions
```
>>> animals = ['dog', 'cat', 'bird', 'fish', 'snake']
>>> animal for animal in animals
'dog' 'cat' 'bird' 'fish' 'snake'

>>> animal for animal in animals if len(animal) > 3
'bird' 'fish' 'snake'
```
## While loop
```
>>> i = 0
>>> while i < 5:
...     print(i, end = ' ')
...     i += 1
0 1 2 3 4
```
