# String

***A string is a series of characters. Anything inside quotes is considered a
string in Python, and you can use single or double quotes around your
strings like this***

>>example
___
"This is a string."

'This is also a string.'
___

> This flexibility allows you to use quotes and apostrophes within your strings:

>>example
___
'I told my friend, "Python is my favorite language!"'

"The language 'Python' is named after Monty Python, not the snake."

"One of Python's strengths is its diverse and supportive community."
___

## using strings in  variables  
```python

first_name = "chamara"
last_name = "Weerasinghe"
full_name = f"{first_name} {last_name}"

print(full_name)
```
***To insert a `variable`’s value into a `string`, place the letter `f `immediately
before the opening quotation mark ➊. Put braces around the name or names
of any variable you want to use inside the string. Python will replace each
variable with its value when the string is displayed.
These strings are called `f-strings`. The f is for format, because Python
formats the string by replacing the name of any variable in braces with its
value. The output from the previous code is:***

>> F-string example

```python

print(f"Hello, {full_name.title()}!")

```

___
## Adding Whitespace to Strings with Tabs or Newlines
***In programming, whitespace refers to any nonprinting character, such as
spaces, tabs, and end-of-line symbols. You can use whitespace to organize
your output so it’s easier for users to read.***
>> example
```python
print("python")
print("\tpython")

```
> output
```python
python
	python
```

***You can also combine tabs and newlines in a single string. The string
"\n\t" tells Python to move to a new line, and start the next line with a tab.***

```python

 print("Languages:\n\tPython\n\tC\n\tJavaScript")

```
```python

Languages:
Python
C
JavaScript

```

## Stripping Whitespace

***Extra whitespace can be confusing in your programs. To programmers
'python' and 'python ' look pretty much the same. But to a program, they are
two different strings. Python detects the extra space in 'python ' and
considers it significant unless you tell it otherwise.
It’s important to think about whitespace, because often you’ll want to
compare two strings to determine whether they are the same. For example,
one important instance might involve checking people’s usernames when
they log in to a website. Extra whitespace can be confusing in much simpler
situations as well. Fortunately, Python makes it easy to eliminate extraneous
whitespace from data that people enter.
Python can look for extra whitespace on the right and left sides of a
string. To ensure that no whitespace exists at the right end of a string, use
the rstrip() method.***

>> example 


```python

 >>> favorite_language = 'python '
 >>> favorite_language
'python '
 >>> favorite_language.rstrip()
'python'
 >>> favorite_language
'python '

```

***To remove the whitespace from the string permanently, you have to
associate the stripped value with the variable name:***

>> example 
```python

>>> favorite_language = 'python '
>>> favorite_language = favorite_language.rstrip()
>>> favorite_language
'python'

```

***You can also strip whitespace from the left side of a string using the
lstrip() method, or from both sides at once using strip():***
>> example 
```python
>>> favorite_language = ' python '
>>> favorite_language.rstrip()
' python'
>>> favorite_language.lstrip()
'python '
>>> favorite_language.strip()
'python'

```

___

[String.py](../String.py)
> output
```python
"E:\Code\python\python book 2nd eddition\chapter one\venv\Scripts\python.exe" "E:/Code/python/python book 2nd eddition/chapter one/String.py"
Ada Lovelace
ADA LOVELACE
ada lovelace

```