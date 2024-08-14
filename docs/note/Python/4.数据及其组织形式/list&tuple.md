**列表 `list`**

Python 内置的一种数据类型是列表。`list` 是一种类似于向量的结构，可以随时添加和删除其中的元素。

```python
>>> a = [2, 3] # Init a list

>>> a.append(4) # Append elements to list
>>> a
[2, 3, 4]

>>> b = ['a', 'c', 114514]
>>> b
['a', 'c', 114514]

>>> a + b # List "plus"
[2, 3, 4, 'a', 'c', 114514]

>>> a[0] = "c7w,yyds" # Change value of elements
>>> a
['c7w,yyds', 3, 4]

>>> a[-1] # Find the last element
4

>>> a.reverse() # Reverse the list
>>> a
[4, 3, 'c7w,yyds']

>>> p = [5, 4, 3, 2, 1]
>>> p.sort() # Sort the list
>>> p
[1, 2, 3, 4, 5]
```

- list元素也可以是另一个list，ps:多维数组这不就来了吗

**元组 `tuple`**

Python 的元组与列表类似，不同之处在于元组的元素不能修改。元组使用小括号，列表使用方括号。

元组创建很简单，只需要在括号中添加元素，并使用逗号隔开即可。

```python
tup1 = () # 空元组
tup1 = (50, ) # 元组中只包含一个元素时，需要在元素后面添加逗号，来消除歧义
tup1[0] = 20 # Error! Elements of tuple cannot be changed.
```