# **LISTS**

## **What Is a List?**
***A list is a collection of items in a particular order. You can make a list that
includes the letters of the alphabet, the digits from 0–9, or the names of all
the people in your family. You can put anything you want into a list, and the
items in your list don’t have to be related in any particular way. Because a list
usually contains more than one element, it’s a good idea to make the name of
your list plural, such as letters, digits, or names.***

***In Python, `square brackets ([]) `indicate a list, and individual elements in
the list are separated by commas. Here’s a simple example of a list that
contains a few kinds of bicycles:***
```python
bicycles = ['trek', 'cannondale', 'redline', 'specialized']
print(bicycles)
```
```python
['trek', 'cannondale', 'redline', 'specialized']
```
## **Accessing Elements in a List**
***Lists are ordered collections, so you can access any element in a list by
telling Python the position, or index, of the item desired. To access an
element in a list, write the name of the list followed by the index of the item
enclosed in square brackets.***
```python
print(bicycles[0])
print(bicycles[1])
print(bicycles[2])
```
```python
trek
cannondale
redline
```

## **Index Positions Start at 0, Not 1**
***Python considers the first item in a list to be at position 0, not position 1.
This is true of most programming languages, and the reason has to do with
how the list operations are implemented at a lower level. If you’re receiving
unexpected results, determine whether you are making a simple off-by-one
error.***
```python
bicycles = ['trek', 'cannondale', 'redline', 'specialized']
print(bicycles[1])
print(bicycles[3])

output->
------------
cannondale
specialized

```

## **Last Element Of An Array**
***Python has a special syntax for accessing the last element in a list. By
asking for the item at index -1, Python always returns the last item in the list:***
```python
bicycles = ['trek', 'cannondale', 'redline', 'specialized']
print(bicycles[-1])

output->
------------
specialized
```

## **Using Individual Values from a List**
***You can use individual values from a list just as you would any other variable.
For example, you can use f-strings to create a message based on a value from
a list.***
```python
bicycles = ['trek', 'cannondale', 'redline', 'specialized']
message = f"My first bicycle was a {bicycles[0].title()}."
print(message)
```
```python
My first bicycle was a Trek.

```
## ****
******
```python

```

## ****
******
```python

```

## ****
******
```python

```

## ****
******
```python

```

## ****
******
```python

```