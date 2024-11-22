# Expressions and Variables in Python

## 1. Introduction to Variables and Expressions

In Python, variables are used to store data that can be referenced and manipulated throughout a program. An **expression** is a combination of variables, constants, and operators that Python can evaluate to produce a value. Understanding how to use variables and expressions is crucial for writing effective Python programs.

### Variables in Python

A **variable** is essentially a name that refers to a value or object in memory. Variables are dynamically typed in Python, meaning you do not need to declare their type when you create them; Python will infer the type based on the assigned value.

```python
x = 10  # Variable x is assigned the value 10
name = "Alice"  # Variable name is assigned a string
```

### Expression in Python

An **expression** is any combination of values, variables, operators, and functions that Python evaluates to produce a value. Expressions can be simple or complex, and they can involve multiple data types, operations, and functions.

```python
# Simple arithmetic expression
x = 5 + 3  # x will hold the value 8

# More complex expression
result = (2 * 3) + (4 / 2)  # result will hold the value 8.0
```

## 2. Types of Expressions

### 2.1 Arithmetic Expressions

Arithmetic expressions involve mathematical operations such as addition, subtraction, multiplication, and division. These expressions return a numeric result.

**Example:**

```python
x = 10 + 5   # Addition
y = 10 - 5   # Subtraction
z = 10 * 5   # Multiplication
a = 10 / 5   # Division (float)
b = 10 // 3  # Floor division (integer result)
c = 10 % 3   # Modulo (remainder)
d = 2 ** 3   # Exponentiation (2 raised to the power of 3)
```

### 2.2 Comparison Expressions

Comparison expressions are used to compare two values and return a boolean (`True` or `False`) based on the result. The operators used for comparisons include `==`, `!=`, `<`, `>`, `<=`, and `>=`.

**Example:**

```python
x = 5
y = 10

result = x < y   # result is True
result2 = x == y  # result2 is False
result3 = x != y  # result3 is True
```

### 2.3 Logical Expressions

Logical expressions are used to combine boolean values using logical operators: `and`, `or`, and `not`.

**Example:**

```python
x = True
y = False

result = x and y  # result is False
result2 = x or y  # result2 is True
result3 = not x   # result3 is False
```

### 2.4 String Expressions

String expressions are operations that involve manipulating or combining strings. Common operations include concatenation, repetition, and slicing.

**Example:**

```python
# Concatenation (joining two strings)
greeting = "Hello, " + "world!"  # greeting is "Hello, world!"

# Repetition (repeating a string multiple times)
repeat = "Python " * 3  # repeat is "Python Python Python "

# Slicing (extracting a portion of a string)
text = "Hello, Python"
substring = text[0:5]  # substring is "Hello"
```

## 3. Variables and Assignments

In Python, variables are assigned values using the **assignment operator** (`=`). Once a variable is assigned a value, you can use it in expressions, and the value can be updated at any time.

### 3.1 Simple Assignment

In simple assignment, you assign a value directly to a variable.

**Example:**

```python
x = 10  # x is now 10
y = 20  # y is now 20
```

### 3.2 Multiple Assignments

Python allows multiple variables to be assigned values in a single line.

**Example:**

```python
a, b, c = 1, 2, 3  # a is 1, b is 2, c is 3
```

### 3.3 Swapping Values

You can also swap the values of two variables in Python in a single line.

**Example:**

```python
a = 5
b = 10

# Swapping values
a, b = b, a  # a is now 10, b is now 5
```

### 3.4 Updating Variables

Once a variable is assigned a value, you can update its value by reassigning it.

**Example:**

```python
x = 5
x = x + 3  # x is now 8
x += 2      # x is now 10
x *= 2      # x is now 20
```

## 4. Expressions in Python

An expression is any combination of variables, constants, and operators that evaluates to a value. The result of an expression can be stored in a variable for later use.

### 4.1 Evaluating Expressions

You can evaluate expressions directly in Python using the interactive shell or in a script.

**Example:**

```python
# Evaluating a simple expression
result = 10 + 5  # result is 15

# More complex expressions
expression = (2 * 5) + (10 / 2)  # result is 15.0
```

### 4.2 Expressions with Functions

You can also include function calls within expressions. For example, using the `max()` function to get the maximum of two numbers.

**Example:**

```python
x = 5
y = 10
max_value = max(x, y)  # max_value is 10
```

## 5. Expressions in Conditional Statements

Expressions are often used in conditional statements (like `if`, `elif`, and `else`) to make decisions based on boolean values.

**Example:**

```python
x = 10
y = 20

if x < y:  # This is an expression
    print("x is smaller than y")
else:
    print("x is not smaller than y")
```

## 6. Summary and Table of Operators

| Operator     | Type of Operation                    | Example                     |
|--------------|--------------------------------------|-----------------------------|
| `+`          | Addition                             | `5 + 3 = 8`                 |
| `-`          | Subtraction                          | `5 - 3 = 2`                 |
| `*`          | Multiplication                       | `5 * 3 = 15`                |
| `/`          | Division (float result)              | `5 / 2 = 2.5`               |
| `//`         | Floor Division (integer result)      | `5 // 2 = 2`                |
| `%`          | Modulo (remainder)                   | `5 % 2 = 1`                 |
| `**`         | Exponentiation (power)               | `2 ** 3 = 8`                |
| `==`         | Equal to                             | `5 == 3` is `False`         |
| `!=`         | Not equal to                         | `5 != 3` is `True`          |
| `<`          | Less than                            | `5 < 3` is `False`          |
| `>`          | Greater than                         | `5 > 3` is `True`           |
| `<=`         | Less than or equal to                | `5 <= 3` is `False`         |
| `>=`         | Greater than or equal to             | `5 >= 3` is `True`          |
| `and`        | Logical AND                          | `True and False` is `False` |
| `or`         | Logical OR                           | `True or False` is `True`   |
| `not`        | Logical NOT                          | `not True` is `False`       |

---
