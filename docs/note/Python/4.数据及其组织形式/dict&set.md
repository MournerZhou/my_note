**字典 `dict`**

字典是另一种可变容器模型，且可存储任意类型对象，采用**键值对**存储方式。

字典的每个键值对用冒号 `:` 分割，每个键值对之间用逗号 `,` 分割，整个字典包括在花括号 `{}` 中。

```python
>>> d = {'name': 'c7w', 'gender': 'M', 'id': 2020000000} # Init the dict
>>> d
{'name': 'c7w', 'gender': 'M', 'id': 2020000000}

>>> d['gender'] # Get the value of certain key
'M'

>>> d['department'] = 'CST' # New a key-value pair
>>> d
{'name': 'c7w', 'gender': 'M', 'id': 2020000000, 'department': 'CST'}

>>> d['girlfriend'] # Would raise KeyError if key not found
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
KeyError: 'girlfriend'

>>> d['id'] += 2 # Change value of certain key
>>> d
{'name': 'c7w', 'gender': 'M', 'id': 2020000002, 'department': 'CST'}
```

可以使用 `in` 关键字判断某个特定的 key 是否在字典中，也可以使用内置的 `dictObj.get()` 函数在 key 不存在时提供默认获取值。
要避免key不存在的错误，有两种办法，一是通过`in`判断key是否存在：

```
>>> 'Thomas' in d
False
```

二是通过dict提供的`get()`方法，如果key不存在，可以返回`None`，或者自己指定的value：

```
>>> d.get('Thomas')
>>> d.get('Thomas', -1)
-1
```

注意：返回`None`的时候Python的交互环境不显示结果。

要删除一个key，用`pop(key)`方法，对应的value也会从dict中删除：

```
>>> d.pop('Bob')
75
>>> d
{'Michael': 95, 'Tracy': 85}
```

请务必注意，dict内部存放的顺序和key放入的顺序是没有关系的。

和list比较，dict有以下几个特点：

1. 查找和插入的速度极快，不会随着key的增加而变慢；
2. 需要占用大量的内存，内存浪费多

**集合 `set`**

`set` 和 `dict` 类似，也是一组 key 的集合，但不存储 value。由于 key 不能重复，所以，在 `set` 中，没有重复的 key。

```python
>>> myList = [1, 1, 1, 2, 3, 3, 3, 3, 4]
>>> s = set(myList)
>>> s
{1, 2, 3, 4}
>>> s = list(s)
>>> s
[1, 2, 3, 4]
```