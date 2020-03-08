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

## **Removing Elements from a List**
***Often, you’ll want to remove an item or a set of items from a list. For
example, when a player shoots down an alien from the sky, you’ll most likely
want to remove it from the list of active aliens. Or when a user decides to
cancel their account on a web application you created, you’ll want to remove
that user from the list of active users. You can remove an item according to
its position in the list or according to its value.***


## **Removing an Item Using the del Statement**
***If you know the position of the item you want to remove from a list, you can
use the del statement.***
```python
motorcycles = ['honda', 'yamaha', 'suzuki']
print(motorcycles)
del motorcycles[0]
print(motorcycles)

del motorcycles[1]
print(motorcycles)

```
```python
['honda', 'yamaha', 'suzuki']
['yamaha', 'suzuki']

['honda', 'yamaha', 'suzuki']
['honda', 'suzuki']

```

## **Removing an Item Using the pop() Method**
***Sometimes you’ll want to use the value of an item after you remove it from a
list. For example, you might want to get the x and y position of an alien that
was just shot down, so you can draw an explosion at that position. In a web
application, you might want to remove a user from a list of active members
and then add that user to a list of inactive members.***

***The pop() method removes the last item in a list, but it lets you work with
that item after removing it. The term pop comes from thinking of a list as a
stack of items and popping one item off the top of the stack. In this analogy,
the top of a stack corresponds to the end of a list.***
```python
motorcycles = ['honda', 'yamaha', 'suzuki']
print(motorcycles)
popped_motorcycle = motorcycles.pop()
print(motorcycles)
print(popped_motorcycle)
```
```python
['honda', 'yamaha', 'suzuki']
['honda', 'yamaha']
suzuki
```

***
How might this pop() method be useful? Imagine that the motorcycles in
the list are stored in chronological order according to when we owned them.
If this is the case, we can use the pop() method to print a statement about the
last motorcycle we bought:
***

```python
motorcycles = ['honda', 'yamaha', 'suzuki']
last_owned = motorcycles.pop()
print(f"The last motorcycle I owned was a {last_owned.title()}.")
```

```python
The last motorcycle I owned was a Suzuki.
```

# **Popping Items from any Position in a List**
***You can use pop() to remove an item from any position in a list by including
the index of the item you want to remove in parentheses.***
```python
motorcycles = ['honda', 'yamaha', 'suzuki']
first_owned = motorcycles.pop(0)
print(f"The first motorcycle I owned was a {first_owned.title()}.")
```
```python
The first motorcycle I owned was a Honda.
```

# **Removing an Item by Value**
***Sometimes you won’t know the position of the value you want to remove
from a list. If you only know the value of the item you want to remove, you
can use the remove() method.***
```python
motorcycles = ['honda', 'yamaha', 'suzuki', 'ducati']
print(motorcycles)
motorcycles.remove('ducati')
print(motorcycles)
```
```python

['honda', 'yamaha', 'suzuki', 'ducati']
['honda', 'yamaha', 'suzuki']

```
`The remove() method deletes only the first occurrence of the value you specify. If
there’s a possibility the value appears more than once in the list, you’ll need to
use a loop to make sure all occurrences of the value are removed.`
# **Organizing a List**
***Often, your lists will be created in an unpredictable order, because you can’t
always control the order in which your users provide their data. Although
this is unavoidable in most circumstances, you’ll frequently want to present
your information in a particular order. Sometimes you’ll want to preserve
the original order of your list, and other times you’ll want to change the
original order. Python provides a number of different ways to organize your
lists, depending on the situation.***


# **Sorting a List Permanently with the sort() Method**
******
```python
cars = ['bmw', 'audi', 'toyota', 'subaru']
cars.sort()
print(cars)
```
```python
['audi', 'bmw', 'subaru', 'toyota']
```
***You can also sort this list in reverse alphabetical order by passing the
argument reverse=True to the sort() method. The following example sorts the
list of cars in reverse alphabetical order:***
```python
cars = ['bmw', 'audi', 'toyota', 'subaru']
cars.sort(reverse=True)
print(cars)

```
```python
['toyota', 'subaru', 'bmw', 'audi']
```

# **Sorting a List Temporarily with the sorted() Function**
***To maintain the original order of a list but present it in a sorted order, you
can use the sorted() function. The sorted() function lets you display your list
in a particular order but doesn’t affect the actual order of the list.***
```python
cars = ['bmw', 'audi', 'toyota', 'subaru']
print("Here is the original list:")
print(cars)
print("\nHere is the sorted list:")
print(sorted(cars))
print("\nHere is the original list again:")
print(cars)

```
```python
Here is the original list:
['bmw', 'audi', 'toyota', 'subaru']
Here is the sorted list:
['audi', 'bmw', 'subaru', 'toyota']
Here is the original list again:
['bmw', 'audi', 'toyota', 'subaru']
```
***Sorting a list alphabetically is a bit more complicated when all the values are
not in lowercase. There are several ways to interpret capital letters when
determining a sort order, and specifying the exact order can be more complex
than we want to deal with at this time. However, most approaches to sorting
will build directly on what you learned in this section.***

# **Printing a List in Reverse Order**
***To reverse the original order of a list, you can use the reverse() method. If we
originally stored the list of cars in chronological order according to when we
owned them, we could easily rearrange the list into reverse chronological
order:***
```python
cars = ['bmw', 'audi', 'toyota', 'subaru']
print(cars)
cars.reverse()
print(cars)

```
```python
['bmw', 'audi', 'toyota', 'subaru']
['subaru', 'toyota', 'audi', 'bmw']
```
***The reverse() method changes the order of a list permanently, but you can
revert to the original order anytime by applying reverse() to the same list a
second time.***
# **Finding the Length of a List**
***You can quickly find the length of a list by using the len() function.***
```python
>>> cars = ['bmw', 'audi', 'toyota', 'subaru']
>>> len(cars)
4

```
***Python counts the items in a list starting with one, so you shouldn’t run into any
of -by-one errors when determining the length of a list.***
# **Avoiding Index Errors When Working with Lists**
***One type of error is common to see when you’re working with lists for the
first time. Let’s say you have a list with three items, and you ask for the
fourth item:***
```python
motorcycles = ['honda', 'yamaha', 'suzuki']
print(motorcycles[3])

motorcycles = []
print(motorcycles[-1])


```
```python
Traceback (most recent call last):
File "motorcycles.py", line 2, in <module>
print(motorcycles[3])
IndexError: list index out of range

Traceback (most recent call last):
File "motorcyles.py", line 3, in <module>
print(motorcycles[-1])
IndexError: list index out of range

```

***If an index error occurs and you can’t figure out how to resolve it, try printing
your list or just printing the length of your list. Your list might look much
dif erent than you thought it did, especially if it has been managed dynamically
by your program. Seeing the actual list, or the exact number of items in your
list, can help you sort out such logical errors.***
