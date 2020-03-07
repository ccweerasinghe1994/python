#Variables
1.   Variable names can contain only letters, numbers, and underscores.
They can start with a letter or an underscore, but not with a number.
For instance, you can call a variable message_1 but not 1_message.
1.  Spaces are not allowed in variable names, but underscores can be used
to separate words in variable names. For example, greeting_message
works, but greeting message will cause errors.
1.  Avoid using Python keywords and function names as variable names;
that is, do not use words that Python has reserved for a particular
programmatic purpose, such as the word print. (See “Python Keywords
and Built-in Functions” on page 471.)
1.  Variable names should be short but descriptive. For example, name is
better than n, student_name is better than s_n, and name_length is better
than length_of_persons_name.
1.  Be careful when using the lowercase letter l and the uppercase letter O
because they could be confused with the numbers 1 and 0.
>code
```python
message = "hello world python"
print(message)
```
> output

```bash
hello python interpreter
hello world python
```

[Code](../intro.py)