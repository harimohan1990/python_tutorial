# Python Basics - Section 1: Fundamentals

Welcome to the fundamentals of Python! In this section, we’ll walk you through the essential building blocks of Python programming, perfect for beginners who are starting from scratch.

---

## 1. Python Syntax

Python emphasizes readability and simplicity.

### Example:

```python
print("Hello, World!")
```

* No semicolons needed.
* Indentation (typically 4 spaces) defines code blocks.
* Case-sensitive.

---

## 2. Variables in Python

Variables store data. You don’t need to declare a type explicitly.

### Example:

```python
name = "Alice"
age = 30
height = 5.6
```

* Variable names should be meaningful.
* Must start with a letter or underscore, not a number.

---

## 3. Strings

Strings are sequences of characters.

### String Creation:

```python
s1 = 'Hello'
s2 = "World"
s3 = '''This is a
multiline string'''
```

### Common Operations:

```python
name = "Hari"
print(name.upper())     # 'HARI'
print(name.lower())     # 'hari'
print(len(name))        # 4
print(name[1])          # 'a'
```

---

## 4. Numbers

Python supports different number types:

* **int**: Whole numbers
* **float**: Decimal numbers

### Example:

```python
x = 10         # int
y = 3.14       # float
```

### Arithmetic Operators:

```python
+ - * / // % **
```

---

## 5. Booleans

Booleans represent truth values.

```python
is_active = True
is_deleted = False
```

### Falsy Values:

* `None`
* `False`
* `0`, `0.0`
* `''`, `[]`, `{}`, `()`

### Example:

```python
if is_active:
    print("Active")
```

---

## 6. Constants

Python doesn't enforce constants but by convention:

```python
PI = 3.14159
MAX_USERS = 100
```

* Use uppercase letters with underscores.

---

## 7. Comments

Use comments to explain code.

### Example:

```python
# This is a single-line comment
"""
This is a
multi-line comment
"""
```

---

## 8. Type Conversion

Convert between types using built-in functions:

### Example:

```python
age = "25"
age = int(age)

price = 99.99
price_str = str(price)
```

### Common Conversion Functions:

* `int()`
* `float()`
* `str()`
* `bool()`

---

