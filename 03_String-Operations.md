# String Operations in Python

## 1. Introduction to String Operations

In Python, strings are sequences of characters enclosed in single (`'`) or double (`"`) quotes. Python provides a rich set of built-in operations and methods for manipulating strings. These operations allow you to perform tasks such as concatenation, slicing, indexing, formatting, and more.

## 2. Basic String Operations

### 2.1 String Concatenation

**Concatenation** is the process of combining two or more strings into a single string. In Python, you can concatenate strings using the `+` operator.

**Example:**

```python
greeting = "Hello"
name = "Alice"
message = greeting + ", " + name + "!"  # Concatenate strings
print(message)  # output: 'Hello, Alice!'
```

### 2.2 String Repetition

You can **repeat** a string multiple times using the `*` operator.

**Example:**

```python
word = "Python"
repeated_word = word * 3  # Repeat 'Python' 3 times
print(repeated_word)  # output: 'PythonPythonPython'
```

### 2.3 String Length

The **length** of a string (the number of characters it contains) can be determined using the `len()` function.

**Example:**

```python
text = "Hello, Python!"
length = len(text)  # Get the length of the string
print(length)  # output: 14
```

## 3. String Indexing and Slicing

### 3.1 String Indexing

Strings in Python are **indexed** starting from `0`. You can access individual characters in a string using their index inside square brackets (`[]`).

- **Positive indexing** starts from `0` for the first character and increases by one as you move to the right.
- **Negative indexing** starts from `-1` for the last character and decreases by one as you move to the left.

**Example:**

```python
text = "Hello"
first_char = text[0]   # Access the first character
last_char = text[-1]   # Access the last character (negative index)
print(first_char)  # output: 'H'
print(last_char)   # output: 'o'
```

### 3.2 String Slicing

**Slicing** allows you to extract a portion of the string by specifying a **range of indices**. The syntax for slicing is:

```python
string[start:end]
```

- `start` is the starting index (inclusive).
- `end` is the ending index (exclusive).

If `start` or `end` are omitted, Python will use default values:
- `start` defaults to `0` (beginning of the string).
- `end` defaults to the length of the string.

**Example:**

```python
text = "Hello, Python!"
substring = text[0:5]  # Slice from index 0 to 4 (exclusive of 5)
print(substring)  # output: 'Hello'

# Slicing with negative indices
substring2 = text[-7:-1]  # Slice from index -7 to -2
print(substring2)  # output: 'Python'
```

### 3.3 String Stride (Step)

In addition to **start** and **end**, you can also specify a **step** (stride) to skip elements. The syntax is:

```python
string[start:end:step]
```

The **step** determines the interval between characters selected in the slice.

- A **step of 2** will select every second character.
- A **negative step** will reverse the string.

**Example:**

```python
text = "Hello, Python!"
# Select every second character
stride_example = text[0:10:2]  # Slice from 0 to 10, with a step of 2
print(stride_example)  # output: 'Hoo y'

# Reverse the string using a negative step
reversed_text = text[::-1]
print(reversed_text)  # output: '!nohtyP ,olleH'
```

## 4. Escape Sequences

An **escape sequence** is a special sequence of characters that allows you to insert characters that would otherwise be difficult to include in a string, such as newline characters or quotation marks. Escape sequences are prefixed with a backslash (`\`).

### Common Escape Sequences

| Escape Sequence | Description                        | Example       |
|-----------------|------------------------------------|---------------|
| `\'`            | Single quote                        | `\'Hello\'` → `'Hello'` |
| `\"`            | Double quote                        | `\"Hello\"` → `"Hello"` |
| `\\`            | Backslash                           | `\\n` → `\n`  |
| `\n`            | Newline                             | `"Hello\nWorld"` → 'Hello' followed by a new line and 'World' |
| `\t`            | Tab                                 | `"Hello\tWorld"` → 'Hello' followed by a tab space and 'World' |
| `\r`            | Carriage return                     | `"Hello\rWorld"` → 'World' |
| `\b`            | Backspace                           | `"Hello\bWorld"` → 'HellWorld' |

**Example:**

```python
text = "Hello\nPython!"  # Newline escape sequence
print(text)  # output: 'Hello' on the first line and 'Python!' on the second line

quote = "He said, \"Python is awesome!\""  # Escape double quotes
print(quote)  # output: He said, "Python is awesome!"
```

## 5. String Methods

Python provides a variety of built-in string methods for modifying and querying strings.

### 5.1 `.lower()` and `.upper()`

- `.lower()` converts all characters to lowercase.
- `.upper()` converts all characters to uppercase.

**Example:**

```python
text = "Hello, World!"
lower_text = text.lower()  # Convert to lowercase
upper_text = text.upper()  # Convert to uppercase
print(lower_text)  # output: 'hello, world!'
print(upper_text)  # output: 'HELLO, WORLD!'
```

### 5.2 `.strip()`

The `.strip()` method removes any leading (spaces before the text) and trailing (spaces after the text) whitespace from the string.

**Example:**

```python
text = "  Hello, Python!  "
stripped_text = text.strip()  # Remove leading and trailing spaces
print(stripped_text)  # output: 'Hello, Python!'
```

### 5.3 `.replace()`

The `.replace(old, new)` method replaces all occurrences of the substring `old` with the substring `new`.

**Example:**

```python
text = "Hello, World!"
modified_text = text.replace("World", "Python")  # Replace 'World' with 'Python'
print(modified_text)  # output: 'Hello, Python!'
```

### 5.4 `.split()`

The `.split()` method splits a string into a list of substrings based on a delimiter (default is space).

**Example:**

```python
text = "Hello, Python!"
words = text.split()  # Split by spaces (default behavior)
print(words)  # output: ['Hello,', 'Python!']

# Split by a specific delimiter
csv_text = "apple,banana,cherry"
fruits = csv_text.split(",")  # Split by commas
print(fruits)  # output: ['apple', 'banana', 'cherry']
```

### 5.5 `.join()`

The `.join()` method is the reverse of `.split()`. It joins a list of strings into a single string, using the specified separator.

**Example:**

```python
words = ['Hello', 'Python', 'World']
sentence = " ".join(words)  # Join list of words with a space
print(sentence)  # output: 'Hello Python World'
```

### 5.6 `.find()` and `.index()`

Both `.find()` and `.index()` search for a substring in the string. The difference is that `.find()` returns `-1` if the substring is not found, while `.index()` raises a `ValueError` if the substring is not found.

**Example:**

```python
text = "Hello, Python!"
position = text.find("Python")  # Find the position of the substring
print(position)  # output: 7

# Using .index() (raises an error if not found)
position2 = text.index("Python")
print(position2)  # output: 7
```

### 5.7 `.startswith()` and `.endswith()`

These methods check if a string starts or ends with a specific substring.

- `.startswith(substring)` returns `True` if the string starts with `substring`, otherwise `False`.
- `.endswith(substring)` returns `True` if the string ends with `substring`, otherwise `False`.

**Example:**

```python
text = "Hello, Python!"
start_check = text.startswith("Hello")  # Check if it starts with "Hello"
end_check = text.endswith("Python!")   # Check if it ends with "Python!"
print(start_check)  # output: True
print(end_check)    # output: True
```

### 5.8 `.count()`

The `.count(substring)` method

 counts the number of occurrences of `substring` in the string.

**Example:**

```python
text = "apple, banana, apple, cherry"
count = text.count("apple")  # Count occurrences of "apple"
print(count)  # output: 2
```

## 6. String Formatting

### 6.1 Using `f-strings` (Formatted String Literals)

Introduced in Python 3.6, **f-strings** provide a concise way to embed expressions inside string literals. You can embed variables or expressions within curly braces `{}`.

**Example:**

```python
name = "Alice"
age = 30
greeting = f"Hello, {name}. You are {age} years old."
print(greeting)  # output: 'Hello, Alice. You are 30 years old.'
```

### 6.2 Using `.format()`

The `.format()` method allows for more flexibility in string formatting by using placeholders.

**Example:**

```python
greeting = "Hello, {}. You are {} years old.".format("Bob", 25)
print(greeting)  # output: 'Hello, Bob. You are 25 years old.'
```

## 7. Summary and String Methods Table

| Method         | Description                                        | Example                           |
|----------------|----------------------------------------------------|-----------------------------------|
| `.lower()`     | Converts all characters to lowercase               | `"HELLO".lower()` → `'hello'`     |
| `.upper()`     | Converts all characters to uppercase               | `"hello".upper()` → `'HELLO'`     |
| `.strip()`     | Removes leading and trailing whitespace            | `"  hello  ".strip()` → `'hello'` |
| `.replace()`   | Replaces occurrences of a substring                | `"hello".replace("e", "a")` → `'hallo'` |
| `.split()`     | Splits a string into a list of substrings          | `"apple,banana".split(",")` → `['apple', 'banana']` |
| `.join()`      | Joins a list of strings into a single string       | `" ".join(['hello', 'world'])` → `'hello world'` |
| `.find()`      | Finds the first occurrence of a substring          | `"hello".find("e")` → `1`         |
| `.startswith()`| Checks if a string starts with a substring         | `"hello".startswith("he")` → `True` |
| `.endswith()`  | Checks if a string ends with a substring           | `"hello".endswith("lo")` → `True` |
| `.count()`     | Counts occurrences of a substring in the string   | `"hello".count("l")` → `2`        |

---
