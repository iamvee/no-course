# Collections

## famous collections

### `tuple`

#### check type

### `list`

### `dict`

### `set`

## Collection Operators

### `list + list`, `tuple + tuple`, `str + str`

```python
>>> [1, 2, 3] + [5, 6, 7]
[1, 2, 3, 5, 6, 7]
>>> (1, 2, 3) + (5, 6, 7)
(1, 2, 3, 5, 6, 7)
>>> "abc" + "defghijk" + "lmno" + "pqrst" + "uvwxyz"
'abcdefghijklmnopqrstuvwxyz'
```

###  `list * int`, `tuple * int`, `str * int`


### Invalid Operators for collections 
* `list + tuple`

```
>>> (1, 2, 3) + [5, 6, 7]
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: can only concatenate tuple (not "list") to tuple
```

* `dict + dict`

```python
>>> {'a': 100} + {'b':200}
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: unsupported operand type(s) for +: 'dict' and 'dict'
```

* `set - set`
## convert
