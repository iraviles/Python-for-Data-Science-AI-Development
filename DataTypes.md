# Data Types in Python

## 1. Introduction to Data Types in Python

In Python, data types define the nature of values that can be stored and manipulated. Understanding data types is essential for working with variables and data structures. Python is a dynamically-typed language, which means you do not need to declare the type of a variable when creating it.

The main data types in Python are:

- **Numeric**: integers (`int`), floating-point numbers (`float`).
- **Sequences**: strings (`str`), lists (`list`), tuples (`tuple`).
- **Boolean**: `bool` (values `True` and `False`).
- **Collections**: dictionaries (`dict`).
  
We will explore each of these types in detail below.

## 2. Numeric Data Types

### 2.1 Integers (`int`)

An **integer** is a whole number without a decimal point. It can be positive, negative, or zero.

**Example:**

```python
x = 5        # a positive integer
y = -3       # a negative integer
z = 0        # zero is also an integer
```

### 2.2 Floating-Point Numbers (`float`)

A **float** is a number that has a decimal point. It is used to represent real numbers.

**Example:**

```python
a = 3.14     # a positive float
b = -2.5     # a negative float
c = 0.0      # a float representing zero
```

### 2.3 Operations with Numbers

Python supports basic mathematical operations such as addition, subtraction, multiplication, and division.

**Example:**

```python
# Addition
x = 5 + 3  # result: 8

# Subtraction
y = 5 - 3  # result: 2

# Multiplication
z = 5 * 3  # result: 15

# Division (always returns a float)
w = 5 / 2  # result: 2.5

# Integer Division (removes the decimal part)
q = 5 // 2  # result: 2

# Modulo (remainder of the division)
r = 5 % 2   # result: 1

# Exponentiation
p = 2 ** 3  # result: 8
```

### 2.4 More Examples with Numbers

You can also perform other operations, like calculating square roots or using the `math` module.

**Example:**

```python
import math

# Square root
sqrt_val = math.sqrt(16)  # result: 4.0

# Power of 2
power_val = math.pow(2, 3)  # result: 8.0

# Absolute value
abs_val = abs(-10)  # result: 10
```

## 3. String Data Type (`str`)

A **string** is a sequence of characters enclosed in single (`'`) or double (`"`) quotes.

**Example:**

```python
greeting = "Hello, World!"  # a string with double quotes
name = 'Python'             # a string with single quotes
```

### String Methods

Python provides a variety of string methods, such as:

- `.lower()`: Converts the string to lowercase.
- `.upper()`: Converts the string to uppercase.
- `.split()`: Splits the string into a list of words.
- `.replace()`: Replaces a substring with another string.

**Example:**

```python
text = "Hello, Python"

# Convert to lowercase
print(text.lower())  # output: 'hello, python'

# Convert to uppercase
print(text.upper())  # output: 'HELLO, PYTHON'

# Split the string into words
words = text.split()  
print(words)  # output: ['Hello,', 'Python']

# Replace a substring
new_text = text.replace("Python", "World")
print(new_text)  # output: 'Hello, World'
```

## 4. Boolean Data Type (`bool`)

The **boolean** type has two possible values: `True` and `False`. It is used in conditional statements and loops.

**Example:**

```python
is_adult = True
is_child = False

if is_adult:
    print("This person is an adult")
else:
    print("This person is a child")
```

## 5. Composite Data Types

### 5.1 Lists (`list`)

A **list** is an ordered collection of items, which can be of different data types.

**Example:**

```python
fruits = ["apple", "banana", "cherry"]
print(fruits[0])  # output: 'apple'
```

### 5.2 Tuples (`tuple`)

A **tuple** is similar to a list, but it is **immutable** (cannot be modified after creation).

**Example:**

```python
coordinates = (10, 20)
print(coordinates[1])  # output: 20
```

### 5.3 Dictionaries (`dict`)

A **dictionary** is an unordered collection of key-value pairs.

**Example:**

```python
person = {"name": "John", "age": 30}
print(person["name"])  # output: 'John'
```

## 6. Type Casting

Sometimes, you need to convert a value from one data type to another. Python provides functions such as `int()`, `float()`, and `str()` for type casting.

### 6.1 Implicit Type Casting (Automatic)

Python automatically converts data types when required. This is known as implicit type casting.

**Example:**

```python
# Integer to float
x = 5   # integer
y = 2.0 # float
result = x + y  # Python automatically converts x to float
print(result)  # output: 7.0
```

### 6.2 Explicit Type Casting (Manual)

You can manually cast a value from one type to another using type casting functions.

**Example:**

```python
# String to integer
num_str = "123"
num_int = int(num_str)  # converts the string to an integer
print(num_int)  # output: 123

# String to float
num_float = float(num_str)  # converts the string to a float
print(num_float)  # output: 123.0

# Integer to string
num_str2 = str(num_int)  # converts the integer to a string
print(num_str2)  # output: '123'
```

### 6.3 Common Data Type Conversion Examples

**Example 1: Converting a float to an integer (truncates the decimal part):**

```python
float_num = 5.67
int_num = int(float_num)  # converts to integer
print(int_num)  # output: 5
```

**Example 2: Converting a boolean to an integer (`True` becomes 1, `False` becomes 0):**

```python
bool_val = True
int_val = int(bool_val)  # converts to integer
print(int_val)  # output: 1
```

**Example 3: Converting an integer to a boolean (`0` becomes `False`, any non-zero value becomes `True`):**

```python
int_val = 0
bool_val = bool(int_val)  # converts to boolean
print(bool_val)  # output: False
```

## 7. Summary and Data Types Table

| Data Type   | Description                                        | Example                         |
|-------------|----------------------------------------------------|---------------------------------|
| `int`       | Integer values without decimal points              | `5`, `-3`, `0`                  |
| `float`     | Floating-point numbers (with decimal points)       | `3.14`, `-2.5`, `0.0`           |
| `str`       | Sequence of characters                             | `"Hello"`, `'Python'`           |
| `bool`      | Boolean values (`True` or `False`)                 | `True`, `False`                 |
| `list`      | Ordered collection of elements                     | `[1, 2, 3]`, `["a", "b"]`       |
| `tuple`     | Ordered and immutable collection of elements       | `(1, 2, 3)`, `("a", "b")`       |
| `dict`      | Collection of key-value pairs                      | `{"key": "value"}`              |


