# `*`

## multiple variable value assignment

```python
a, b, c = 10, 20, 30
```

### mismatch

```python
>>> a, b, c = 10, 20
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ValueError: not enough values to unpack (expected 3, got 2)
>>> a, b, c = 10, 20, 30, 40 
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ValueError: too many values to unpack (expected 3)
```

## a list for the remaining

```python
>>> a, b, *c = 10, 20, 30, 40 , 50, 60
>>> print(a, b, c)
10 20 [30, 40, 50, 60]
>>> a, *b, c = 10, 20, 30, 40 , 50, 60
>>> print(a, b, c)
10 [20, 30, 40, 50] 60
>>> *a, b, c = 10, 20, 30, 40 , 50, 60
>>> print(a, b, c)
[10, 20, 30, 40] 50 60
```

### only one `*` (to avoid ambiguity)

```python
>>> *a, b, *c = 10, 20, 30, 40 , 50, 60
  File "<stdin>", line 1
SyntaxError: two starred expressions in assignment
```

## call functions 

### unpack collection items and use them as positional argument

```python
>>> inps = (1, 2, 3, 4, 5, 6)
>>> print(1, 2, 3, 4, 5, 6)
1 2 3 4 5 6
>>> print(inps)
(1, 2, 3, 4, 5, 6)
>>> print(*inps)
1 2 3 4 5 6
```
