## String Slicing in Python Explained

String slicing lets you slice into Python strings, and work with their `slices`, or `substrings`—instead of the whole string.

As strings in Python are *immutable*, you cannot change them in place. In this tutorial, you'll learn to slice Python strings and work with substrings.

----


## Python String Slicing Syntax
```py
<str>[start:stop:step]
```
The above line of code:
- Returns a slice of the string `<str>`—starting at index `start`, extending up to `stop-1` in steps of `step`.
- The `start` index is **optional**: the slice starts from the beginning of the string by _default_.
- The `stop` index is also **optional**: the slice extends up to the end of the string by _default_.
- The `step` value is optional too. The default value of step is `1` and includes all characters in the string.

----


## Python String Slicing Example
```py
my_str = "Python3"
```
▶ Let's use `enumerate()` and examine the characters at each index in the string.
```py
for idx,char in enumerate(my_str):
  print(f"At index {idx}: letter {char}")

# Output
At index 0: letter P
At index 1: letter y
At index 2: letter t
At index 3: letter h
At index 4: letter o
At index 5: letter n
At index 6: letter 3
```
In the above code, you've used the `enumerate()` function in conjunction with the `for` loop. This lets you loop through iterables, and access items along with their indices simultaneously—without having to use the `range()` function to get the indices.

▶ Let's now use string slicing.
```py
# With `start` and `stop` indices
print(my_str[1:6])
# Output: ython

# Without `stop` index
print(my_str[1:])
# Output: ython3

# Without `start` index
print(my_str[:5])
# Output: Pytho

# With `step = 2`, slice includes every second character
print(my_str[::2])
# Output: Pto3

# Without `start`, `stop` and `step`: slice is entire string
print(my_str[::])
# Output: Python3
```
----

## Python String Slicing with Negative Step
When you set `step` to a negative value, you can get slices starting from the end of the string—reverse substrings.

If `step = -1` you get a slice starting from the end of the string, and including every character.

This can be super handy when you'd like to _reverse_ a string, like this:
```py
print(my_str[::-1])

# Output: 3nohtyP
```
----

## Conclusion
To sum up, `<str>[start:stop:step]` is the syntax to obtain string slices or substrings in Python.

Now that you've learned how to slice strings, it's time to put your skills to practice, maybe? Happy learning and coding!

