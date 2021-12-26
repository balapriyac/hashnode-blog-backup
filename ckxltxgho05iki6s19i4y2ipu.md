## Python String Methods for Whitespace Removal

When working with Python strings, there are times when you'll need to remove unwanted whitespaces, tabs, and newline characters.

You may have to resize strings, or ensure consistency for further processing - such as processing text collected through forms.

And Python's string methods for whitespace removal return strings with all unwanted whitespaces, and tabs removed.

📑**Note**: I'll use the term whitespaces going forward - whitespaces, tabs, and newlines have all been subsumed in this term 'whitespaces'.

In this tutorial, you'll learn how you can remove leading, trailing, and both leading and trailing whitespaces using the built-in string methods, `lstrip()`, `rstrip()`, and `strip()`, respectively.

## How to Use `lstrip()` to Remove Leading Whitespaces in Python Strings

Let's start with the `lstrip()` method.

> `<string>.lstrip()` returns a copy of the string with all leading whitespaces removed.

The `l` in `lstrip()` stands for left. So this method removes all whitespaces to the left of the first character in the string.
Therefore it removes leading whitespaces.

▶ Here's an example.
Consider the string `"    Coding is hard, yet fun!\t"`  - it has 4 leading whitespaces, and 1 trailing tab (`\t`).

Now, call the `lstrip()` method on this string. And store the returned string in the variable `l_str`.
```py
long_str = "    Coding is hard, yet fun!\t"
l_str = long_str.lstrip()
```
Let's print out the lengths of the original string `long_str`, and the returned string `l_str`.
Now, `l_str` is `"Coding is hard, yet fun!\t"`

```py
print(len(long_str))
print(len(l_str))

# Output
29
25
```
As you can see from the lengths, the 4 leading whitespaces have been removed.

## How to Use `rstrip()` to Remove Trailing Whitespaces in Python Strings

Let's now look at the `rstrip()` method.

>`<string>.rstrip()` returns a copy of the string with all trailing whitespaces removed.

The `r` in `rstrip()` stands for right. So this method removes all whitespaces to the right of the last character in the string.
Therefore it removes trailing whitespaces.

▶ Let's use the same example string from the previous section. And call the `rstrip()` method on this string, store the returned string in the variable `r_str`.

`r_str` is now `"    Coding is hard, yet fun!`

```py
long_str = "    Coding is hard, yet fun!\t"
r_str = long_str.rstrip()
print(len(long_str))
print(len(r_str))

# Output
29
28
```
As you can see, the trailing tab `\t` has been removed. And the returned string's length is one less than the original string—as expected.

## How to Use `strip()` to Remove Leading and Trailing Whitespaces in Python Strings
Now that you know how to remove leading and trailing whitespaces using `lstrip()` and `rstrip()` respectively, in this section, you'll learn how `strip()` method helps remove both leading and trailing whitespaces.

> `<string>.strip()` returns a copy of the string with all leading and trailing whitespaces removed.

▶ As with the earlier sections, let's call the `strip()` method on the string `long_str`.

The resultant string `s_str` is `"Coding is hard, yet fun!"`

```py
long_str = "    Coding is hard, yet fun!\t"
s_str = long_str.strip()
print(len(long_str))
print(len(s_str))

# Output
29
24
```
From the length of the returned string, you can see that both the 4 leading whitespaces, and the trailing `\t` have been removed.

## Conclusion
Hope you found this short tutorial on string methods helpful.

The table below summarizes what you've learned:

|Method|Description|
|---|----|
|`lstrip()`| Returns a copy of the string with all leading whitespaces removed|
|`rstrip()`| Returns a copy of the string with all trailing whitespaces removed|
|`strip()`| Returns a copy of the string with all leading and trailing whitespaces removed|

Happy learning and coding!😄