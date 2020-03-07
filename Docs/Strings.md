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
***To insert a variable’s value into a string, place the letter f immediately
before the opening quotation mark ➊. Put braces around the name or names
of any variable you want to use inside the string. Python will replace each
variable with its value when the string is displayed.
These strings are called f-strings. The f is for format, because Python
formats the string by replacing the name of any variable in braces with its
value. The output from the previous code is:***
>> F-string example
```python
print(f"Hello, {full_name.title()}!")
```



[String.py](../String.py)
> output
```python
"E:\Code\python\python book 2nd eddition\chapter one\venv\Scripts\python.exe" "E:/Code/python/python book 2nd eddition/chapter one/String.py"
Ada Lovelace
ADA LOVELACE
ada lovelace

```