
# Introduction 
Creating a variable in Python, it has a value with a corresponding data type.

There are many different data types, such as:
* integers
* floats
* booleans
* strings 

The above is just a small subset of the available types -there are also:
- dictionaries 
- sets
- lists
- tuples

Data types are important, because they determine what kinds of actions one can do with them.

For instance, `12.0/2.0` makes sense, but "cat"/"dog" does not.

To avoid errors, we need to make sure that the actions match the data types that we have.


# Integers
Are numbers without any fractional part and can be positive (1, 2, 3, ...), negative (-1, -2, -3, ...), or zero (0).


In the code cell below, we set a variable `x` to an integer.

One can verify the data type with `type()`, and need need only pass the variable name into the parentheses.

```bash 
x = 14
print(x)
print(type(x))
```

Ans -> 14
<class 'int'>

In the output above, <class 'int'> refers to the integer data type.


# Float

These are numbers with fractional parts. They can have many numbers after decimal

example 
```bash 
nearly_pi = 3.141592653589793238462643383279502884197169399375105820974944
print(nearly_pi)
print(type(nearly_pi))
```

Ans -> 3.141592653589793
<class 'float'>

Can also specify aq float with a fraction.

```bash 
almost_pi = 22/7
print(almost_pi)
print(type(almost_pi))
```

Ans -> 3.142857142857143
<class 'float'>

One function that is particularly useful for fractions is the `round()` function. It lets one round a number to specified number of decimal places.

example
```bash 
# Round to 5 decimal places
round_pi = round(almost_pi, 5)
print(round_pi)
print(type(round_pi))
```

Ans -> 3.14286
<class 'float'>

Whenever you write an number with a decimal point, Python recognizes it as a float data type.

For instance, `1`. `(or 1.0, 1.00, etc)` will be recognized as a float. This is the case, even though these numbers technically have no fractional part!


example 
```bash 
y_float = 1.
print(y_float)
print(type(y_float))
```

Ans -> 1.0
<class 'float'>


# Booleans
Represents one of two values: `True` or `False`. 

Example
`z_one` is set to a boolean with value `True`.

```bash 
z_one = True 
print(z_one)
print(type(z_one))
```
Ans -> True 
<class 'bool'>

Next, `z_two` is set to a boolean with value `False`.

example
```bash 
z_two = False
print(z_two)
print(type(z_two))
```

False
<class 'bool'>

Booleans are used to represent the truth value of an expression. Since `1 < 2` is a true statement, `z_three` takes on a value of True.

example
```bash 
z_three = (1 < 2)
print(z_three)
print(type(z_three))
```

Ans -> True 
<class 'bool'>


Similarly, since `5 < 3` is a `false statement`, `z_four` takes on a value of False.

example
```bash 
z_four = (5 < 3)
print(z_four)
print(type(z_four))
```

Ans -> False
<class 'bool'>

We can switch the value of a boolean by using not. 

So, `not True` is equivalent to `False`, and `not False` becomes `True`.

example
```bash 
z_five = not z_four 
print(z_five)
print(type(z_five))
```

Ans -> True 
<class 'bool'>


# String 

A collection of characters (like alphabet letters, punctuation, numerical digits, or symbol) contained in quotation marks. 

Strings are commonly used to represent text.

example 
```bash 
w = "Hello, Python!"
print(w)
print(type(w))
```

Ans -> Hello, Python!
<class 'str'>

One can get the length of a string with `len()`. 

"Hello, Python!" has length 14, because it has 14 characters, including the space, comma, and exclamation mark.

Note:
Quotation marks are not included when calculating the length.

example
```bash 
print(len(w))
```

Ans -> 14


One special type of string is the empty string, which has length zero.

example 
```bash 
shortest_sting = ""
print(type(shortest_sting))
print(len(shortest_sting))
```
<class 'str'>
0


If you put a number in quotation marks, it has a string data type.
```bash 
my_number = "1.12321"
print(my_number)
print(type(my_number))
```

Ans -> 1.12321
<class 'str'>


If we have a string that is convertible to a float, we can use `float()`.

This won't always work! 

For instance, we can convert `10.43430` and `3` to floats, but we cannot convert "Hello, Python!" to a float.

```bash 
also_my_number = float(my_number)
print(also_my_number)
print(type(also_my_number))
```

Ans -> 1.12321
<class 'float'>


One can add two numbers (float or integers), one can also add two strings.
It results in a longer string that combines the two original strings by concatenating them.

example

```bash 
new_string = "abc" + "def"
print(new_string)
print(type(new_string))
print(len(new_string))
```
Ans -> abcdef
<class 'str'>


Note that it's not possible to do subtraction or division with two strings. 

One can also can't multiply two strings, but you can multiply a string by an integer. 

This again results in a string that's just the original string concatenated with itself a specified number of times.

example 
```bash 
newest_string = "abc" * 3
print(newest_string)
print(type(newest_string))
```

Ans -> abcabcabc
<class 'str'>


Note that you cannot multiply a string by a float! Trying to do so will return an error.


![alt text](<image-1.png>)

In the error, the "sequence" is the string "abc", and the "non-int of type `float`" is the float (3.).

So, the error message can be reworded to say "can't multiply string by float".



























