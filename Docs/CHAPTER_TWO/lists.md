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
## **Changing, Adding, and Removing Elements**
***Most lists you create will be dynamic, meaning you’ll build a list and then
add and remove elements from it as your program runs its course. For
example, you might create a game in which a player has to shoot aliens out
of the sky. You could store the initial set of aliens in a list and then remove
an alien from the list each time one is shot down. Each time a new alien
appears on the screen, you add it to the list. Your list of aliens will increase
and decrease in length throughout the course of the game.***


## **Modifying Elements in a List**
***The syntax for modifying an element is similar to the syntax for accessing an
element in a list. To change an element, use the name of the list followed by
the index of the element you want to change, and then provide the new value
you want that item to have***
```python
motorcycles = ['honda', 'yamaha', 'suzuki']
print(motorcycles)

motorcycles[0] = 'ducati'
print(motorcycles)
```
```python
['honda', 'yamaha', 'suzuki']
['ducati', 'yamaha', 'suzuki']
```


## **Adding Elements to a List**
***You might want to add a new element to a list for many reasons. For
example, you might want to make new aliens appear in a game, add new data
to a visualization, or add new registered users to a website y***

## **Appending Elements to the End of a List**
***The simplest way to add a new element to a list is to append the item to the
list. When you append an item to a list, the new element is added to the end
of the list. Using the same list we had in the previous example, we’ll add the
new element 'ducati' to the end of the list:***
```python
motorcycles = ['honda', 'yamaha', 'suzuki']
print(motorcycles)
motorcycles.append('ducati')
print(motorcycles)

```
```python
['honda', 'yamaha', 'suzuki']
['honda', 'yamaha', 'suzuki', 'ducati']
```

## **append()**
***The append() method makes it easy to build lists dynamically. For example,
you can start with an empty list and then add items to the list using a series
of append() calls. Using an empty list, let’s add the elements 'honda', 'yamaha',
and 'suzuki' to the list:
***
```python
motorcycles = []
motorcycles.append('honda')
motorcycles.append('yamaha')
motorcycles.append('suzuki')
print(motorcycles)
```
```python
['honda', 'yamaha', 'suzuki']

```

## **Inserting Elements into a List**
***You can add a new element at any position in your list by using the insert()
method. You do this by specifying the index of the new element and the
value of the new item.***
```python
motorcycles = ['honda', 'yamaha', 'suzuki']
➊ motorcycles.insert(0, 'ducati')
print(motorcycles)

```
```python

['ducati', 'honda', 'yamaha', 'suzuki']

```

## **Removing Elements from a List
**
***Often, you’ll want to remove an item or a set of items from a list. For
example, when a player shoots down an alien from the sky, you’ll most likely
want to remove it from the list of active aliens. Or when a user decides to
cancel their account on a web application you created, you’ll want to remove
that user from the list of active users. You can remove an item according to
its position in the list or according to its value.***
```python

```
```python

```

## ****
******
```python

```
```python

```

## ****
******
```python

```
```python

```

