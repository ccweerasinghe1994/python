# **Numbers**

***Numbers are used quite often in programming to keep score in games,
represent data in visualizations, store information in web applications, and so
on. Python treats numbers in several different ways, depending on how
they’re being used. Let’s first look at how Python manages integers, because
they’re the simplest to work with***

## **Integers**


***You can add (+), subtract (-), multiply (*), and divide (/) integers in Python.***

```python

>>> 2 + 3
5
>>> 3 - 2
1
>>> 2 * 3
6
>>> 3 / 2
1.5

```

```python

>>> 3 ** 2
9
>>> 3 ** 3
27
>>> 10 ** 6
1000000

```

**order of operations**

```python

>>> 2 + 3*4
14
>>> (2 + 3) * 4
20

```


## **Floats**

***Python calls any number with a decimal point a float.***

```python
>>> 0.1 + 0.1
0.2
>>> 0.2 + 0.2
0.4
>>> 2 * 0.1
0.2
>>> 2 * 0.2
0.4

```

***But be aware that you can sometimes get an arbitrary number of decimal
places in your answer***


```python

>>> 0.2 + 0.1
0.30000000000000004
>>> 3 * 0.1
0.30000000000000004


```

## **Integers and Floats**

***If you mix an integer and a float in any other operation, you’ll get a float
as well:***

```python
>>> 4/2
2.0
>>> 1 + 2.0
3.0
>>> 2 * 3.0
6.0
>>> 3.0 ** 2
9.0

```
## **Underscores in Numbers**
***Python ignores the underscores when storing these kinds of values. Even
if you don’t group the digits in threes, the value will still be unaffected. To
Python, 1000 is the same as 1_000, which is the same as 10_00. This feature
works for integers and floats, but it’s only available in Python 3.6 and later.***
```python
>>> universe_age = 14_000_000_000
>>> print(universe_age)
14000000000

```
## **Multiple Assignment**

***You can assign values to more than one variable using just a single line***

```python
>>> x, y, z = 0, 0, 0
```


## **Constants**


***A constant is like a variable whose value stays the same throughout the life of
a program. Python doesn’t have built-in constant types, but Python
programmers use all capital letters to indicate a variable should be treated as
a constant and never be changed:***

```python
MAX_CONNECTIONS = 5000
```

