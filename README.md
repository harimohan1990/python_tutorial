### 🟢 **Python Basics**

1. Syntax
2. Variables
3. Strings
4. Numbers
5. Booleans
6. Constants
7. Comments
8. Type Conversion

---

### ➕ **Operators**

9. Arithmetic Operators
10. Assignment Operators
11. Comparison Operators
12. Logical Operators

---

### 🔁 **Control Flow**

13. if…else Statement
14. Ternary Operator
15. for Loop with range()
16. while Loop
17. break
18. continue
19. pass

---

### 🔧 **Functions**

20. Defining Functions
21. Default Parameters
22. Keyword Arguments
23. Recursive Functions
24. Lambda Expressions
25. Docstrings

---

### 📋 **Lists**

26. List Introduction
27. Tuple
28. sort()
29. sorted()
30. Slicing
31. List Unpacking
32. Iterating
33. Indexing
34. Iterables vs Iterators
35. map()
36. filter()
37. reduce()
38. List Comprehensions

---

### 🔑 **Dictionaries**

39. Dictionary
40. Dictionary Comprehension

---

### 🔢 **Sets**

41. Set
42. Set Comprehension
43. Union
44. Intersection
45. Difference
46. Symmetric Difference
47. Subset
48. Superset
49. Disjoint Sets

---

### 🛑 **Exception Handling**

50. try…except
51. try…except…finally
52. try…except…else

---

### 🔂 **More on Loops**

53. for…else
54. while…else
55. do…while Loop Emulation

---

### 🧠 **More on Functions**

56. Unpacking Tuples
57. \*args
58. \*\*kwargs
59. Partial Functions
60. Type Hints

---

### 📦 **Modules & Packages**

61. Modules
62. Module Search Path
63. **name** Variable
64. Packages
65. Private Functions

---

### 📁 **Working with Files**

66. Read Text File
67. Write Text File
68. Create New File
69. Check File Existence
70. Read CSV
71. Write CSV
72. Rename File
73. Delete File

---

### 📂 **Working with Directories**

74. Directory Functions
75. List Files in Directory

---

### 🔤 **Strings**

76. f-Strings
77. Raw Strings
78. Backslash

---

### 📦 **PIP, PyPI & Virtual Environments**

79. PyPI and pip
80. Virtual Environments
81. pipenv on Windows

---

### 🧱 **Python OOP**

82. Object-Oriented Concepts
83. Classes & Objects
84. Class Variables
85. Instance Methods
86. **init**()
87. Instance Variables
88. Private Attributes
89. Class Attributes
90. Static Methods

#### Special Methods

91. **str**
92. **repr**
93. **eq**
94. **hash**
95. **bool**
96. **del**

#### Property

97. @property
98. Read-only Property
99. Delete Property

#### Inheritance

100. Inheritance
101. Method Overriding
102. super()
103. **slots**
104. Abstract Classes

#### Enumeration

105. Enum
106. Enum Aliases & @unique
107. Enum Customization
108. auto

#### SOLID Principles

109. SRP
110. OCP
111. LSP
112. ISP
113. DIP

#### Multiple Inheritance

114. Multiple Inheritance
115. MRO
116. Mixin

#### Descriptors

117. Descriptors
118. Data vs Non-Data Descriptors

#### Metaprogramming

119. **new**
120. type Class
121. Metaclass
122. Metaclass Example
123. dataclass

#### Exceptions in OOP

124. Raising Exceptions
125. Raise from Cause
126. Custom Exceptions

---

### ⚙️ **Python Concurrency**

127. Processes vs Threads
128. threading Module
129. Extending Thread
130. Returning from Thread
131. Multithreading Example
132. Daemon Threads
133. Thread Pools

#### Thread Synchronization

134. Lock
135. Event
136. Stop Thread
137. Semaphore

#### Sharing Data

138. Thread-safe Queue

#### Multiprocessing

139. multiprocessing Module
140. Process Pool

#### Async I/O

141. Event Loop
142. async/await
143. Creating Tasks
144. Canceling Tasks
145. Timeout Cancellation
146. asyncio.wait()
147. Future
148. asyncio.gather()

---

### 🧠 **Advanced Python**

149. References
150. Garbage Collection
151. Dynamic Typing
152. Mutable & Immutable
153. `is` Operator
154. None

#### Variable Scope

155. Built-in, Local, Global
156. nonlocal

#### Closures & Decorators

157. Closures
158. Decorators
159. Decorators with Arguments
160. Class Decorators
161. Monkey Patching

#### Named Tuples

162. namedtuple

#### Sequence Types

163. Sequences
164. Lists vs Tuples
165. Slicing
166. Custom Sequence Type

#### Iterators & Iterables

167. Iterators
168. Iterators vs Iterables
169. iter()

#### Generators

170. Generator Functions
171. Generator Expressions

#### Context Managers

172. Context Manager

#### Integer & Boolean

173. Integer Internals
174. Floor Division (//)
175. Modulo (%)
176. bool
177. `and`
178. `or`

#### Float

179. Float Internals
180. float to int
181. Rounding

#### Decimal

182. Decimal Module


#### 1. Syntax

* Python uses indentation (spaces or tabs) to define code blocks—no `{}` or `end`.
* A colon (`:`) starts suites (after `if`, `for`, `def`, etc.).
* Statements end at the newline; use `\` to wrap or parentheses for implicit line-continuation.

```python
if score >= 90:
    print("A grade")     # indented block
```

---

#### 2. Variables

* Declared by simple assignment; they’re **labels** pointing to objects.
* Dynamic typing: the object (not the variable) has the type, so labels can re-point.
* Naming: letters, digits, `_`, no starting with a digit; case-sensitive.

```python
age = 30
age = "thirty"   # now points to a str object
```

---

#### 3. Strings

* Immutable sequences of Unicode characters (`str`).
* Quote with `'` or `"`, triple-quotes for multi-line / docstrings.
* Common ops: slicing, concatenation (`+`), repetition (`*`), f-strings for interpolation.

```python
name = "Hari"
greet = f"Hi, {name.upper()}!"   # f-string, methods
```

---

#### 4. Numbers

* **int** (unbounded precision) and **float** (64-bit IEEE-754) are core; **complex** for `a + bj`.
* Arithmetic: `+ - * / // % **`; `//` is floor-division, `%` modulus.
* `decimal.Decimal` and `fractions.Fraction` for exact precision use-cases.

```python
pi  = 3.14159
area = pi * (r := 5) ** 2    # walrus operator assigns & uses r
```

---

#### 5. Booleans

* Only two instances: `True`, `False`—subclasses of `int` (`True == 1`).
* Truthiness: 0, `0.0`, `''`, `[]`, `{}`, `None`, and custom objects with `__bool__`→`False`.
* Logical operators: `and`, `or`, `not` (short-circuit evaluation).

```python
if items and not error:
    process(items)
```

---

#### 6. Constants

* No true constant keyword; by convention use ALL\_CAPS names at module level.
* `typing.Final` (PEP 591) signals “don’t reassign” to type checkers.

```python
from typing import Final
API_URL: Final = "https://api.example.com"
```

---

#### 7. Comments

* Single-line: `# explain something`.
* Inline: place after two spaces—`total = x + y  # sum inputs`.
* Docstrings (`"""Triple quoted"""`) are first statements in modules, classes, functions; accessible via `help()`.

```python
def add(a, b):
    """Return the sum of a and b."""
    return a + b
```

---

#### 8. Type Conversion

* **Implicit**: `int` ➝ `float` in mixed arithmetic.
* **Explicit / casting**: built-ins like `int()`, `float()`, `str()`, `bool()`.
* Containers: `list(iterable)`, `tuple()`, `set()`, `dict()` (from key-value pairs).

```python
num_str = "42"
result  = int(num_str) + 8   # 50
```

Below is a crisp cheat-sheet on Python’s operator groups with mini-snippets for instant testing.

---

#### 9. Arithmetic Operators

| Symbol         | Meaning                  | Example                               |
| -------------- | ------------------------ | ------------------------------------- |
| `+`            | addition / concatenation | `3 + 4   # 7`                         |
| `-`            | subtraction              | `9 - 2   # 7`                         |
| `*`            | multiplication / repeat  | `5 * 2   # 10`, `"ha"*3` → `"hahaha"` |
| `/`            | true division (float)    | `7 / 2   # 3.5`                       |
| `//`           | floor division           | `7 // 2  # 3`                         |
| `%`            | modulus (remainder)      | `7 % 2   # 1`                         |
| `**`           | exponentiation           | `2 ** 3  # 8`                         |
| unary `+`, `-` | identity / negation      | `-5`                                  |

---

#### 10. Assignment Operators

Start with `=` and combine with arithmetic (or bitwise) ops to update a variable in-place:

```python
x = 10      # simple assign
x += 3      # x = x + 3      → 13
x -= 2      # x = x - 2      → 11
x *= 4      # x = x * 4      → 44
x /= 11     # x = x / 11     → 4.0
x //= 2     # floor-divide   → 2.0
x %= 2      # modulus        → 0.0
x **= 5     # power          → 0.0
# Also: &=, |=, ^=, >>=, <<= for bitwise updates
```

---

#### 11. Comparison Operators

Return `True` / `False`; support chaining (`a < b < c`).

| Symbol               | Test                 | Example                 |
| -------------------- | -------------------- | ----------------------- |
| `==`, `!=`           | equality, inequality | `5 == 5` → `True`       |
| `>`, `<`, `>=`, `<=` | greater / less       | `3 <= 2` → `False`      |
| `is`, `is not`       | object identity      | `a is b`                |
| `in`, `not in`       | membership           | `'a' in 'cat'` → `True` |

```python
score = 92
print(90 <= score < 100)   # True (chained)
```

---

#### 12. Logical Operators

Combine truthy/falsey expressions; **short-circuit** evaluation.

```python
logged_in = True
is_admin  = False

# and: both must be true
if logged_in and is_admin:
    access = "full"
# or: first truthy wins
status = is_admin or "regular user"   # "regular user"
# not: boolean negation
print(not logged_in)  # False
```


---

#### 13. `if … elif … else`

* Choose code paths based on Boolean expressions.
* First true branch runs; remaining tests are skipped.

```python
temp = 32
if temp < 0:
    print("Freezing")
elif temp < 20:
    print("Cold")
else:
    print("Warm")
```

---

#### 14. Ternary (Conditional) Expression

`<expr1> if <cond> else <expr2>`—inline alternative to `if…else`.

```python
age   = 17
status = "adult" if age >= 18 else "minor"
```

---

#### 15. `for` Loop + `range()`

Iterates over any iterable; `range(start, stop, step)` yields numbers lazily.

```python
for i in range(1, 6):     # 1‒5
    print(i, end=" ")
```

---

#### 16. `while` Loop

Repeats while the condition stays true. Make sure it eventually flips to avoid infinite loops.

```python
n = 5
while n > 0:
    print(n)
    n -= 1
```

---

#### 17. `break`

Exits the nearest enclosing loop immediately.

```python
for num in range(10):
    if num == 3:
        break           # stops at 3
    print(num)
```

---

#### 18. `continue`

Skips the rest of the current iteration and proceeds to the next one.

```python
for char in "banana":
    if char == 'a':
        continue        # skip 'a'
    print(char)         # prints b n n
```

---

#### 19. `pass`

No-op placeholder where a statement is syntactically required (e.g., empty blocks or stub functions).

```python
def todo():             # to implement later
    pass
```

---


Below is a compact refresher on Python control-flow constructs with quick snippets you can drop into a REPL.

---

#### 13. `if … elif … else`

* Choose code paths based on Boolean expressions.
* First true branch runs; remaining tests are skipped.

```python
temp = 32
if temp < 0:
    print("Freezing")
elif temp < 20:
    print("Cold")
else:
    print("Warm")
```

---

#### 14. Ternary (Conditional) Expression

`<expr1> if <cond> else <expr2>`—inline alternative to `if…else`.

```python
age   = 17
status = "adult" if age >= 18 else "minor"
```

---

#### 15. `for` Loop + `range()`

Iterates over any iterable; `range(start, stop, step)` yields numbers lazily.

```python
for i in range(1, 6):     # 1‒5
    print(i, end=" ")
```

---

#### 16. `while` Loop

Repeats while the condition stays true. Make sure it eventually flips to avoid infinite loops.

```python
n = 5
while n > 0:
    print(n)
    n -= 1
```

---

#### 17. `break`

Exits the nearest enclosing loop immediately.

```python
for num in range(10):
    if num == 3:
        break           # stops at 3
    print(num)
```

---

#### 18. `continue`

Skips the rest of the current iteration and proceeds to the next one.

```python
for char in "banana":
    if char == 'a':
        continue        # skip 'a'
    print(char)         # prints b n n
```

---

#### 19. `pass`

No-op placeholder where a statement is syntactically required (e.g., empty blocks or stub functions).

```python
def todo():             # to implement later
    pass
```

---

Below is a tight, copy-ready rundown of Python function essentials—each point shows the syntax rule plus a mini-snippet you can test instantly.

---

#### 20. **Defining Functions**

* Use `def name(params):` and return with `return` (omitted → `None`).

```python
def add(a, b):
    return a + b
```

---

#### 21. **Default Parameters**

* Assign a value in the signature; evaluated **once** at function-definition time.
* Beware of mutable defaults—use `None` + inside fix.

```python
def greet(name, salutation="Hi"):
    return f"{salutation}, {name}!"        # greet("Hari") → "Hi, Hari!"
```

---

#### 22. **Keyword (Named) Arguments**

* Call by `param=value`, order-independent after any positional args.
* Combine `*` and `**` for arbitrary extra args.

```python
def power(base, exp):
    return base ** exp
power(exp=3, base=2)      # 8
```

---

#### 23. **Recursive Functions**

* A function that calls itself; must converge toward a base case.

```python
def factorial(n):
    return 1 if n == 0 else n * factorial(n-1)
```

---

#### 24. **Lambda (Anonymous) Expressions**

* `lambda params: expression` → returns a callable, typically one-liner.
* Great for `key=` or quick inline logic; limited to a single expression.

```python
square = lambda x: x * x
numbers.sort(key=lambda x: x[1])   # sort by 2nd element
```

---

#### 25. **Docstrings**

* Triple-quoted string **immediately** following def/class/module header.
* Shows up in `help(obj)` and tooling; use one-line summary + details.

```python
def add(a, b):
    """Return the sum of a and b.

    Parameters
    ----------
    a, b : numbers
        Values to add.
    """
    return a + b
```

---

Here’s a **detailed explanation** of each concept under **📋 Lists** with clear examples:

---

### 26. **List Introduction**

* A list is an **ordered**, **mutable** collection of elements.
* Defined using square brackets `[]`.

```python
fruits = ["apple", "banana", "cherry"]
fruits.append("mango")  # Adds to the end
print(fruits[0])        # Access first item
```

---

### 27. **Tuple**

* A **tuple** is an **ordered**, **immutable** sequence.
* Created using parentheses `()`.

```python
person = ("Hari", 30)
# person[0] = "John"  → Error: Tuples can't be modified
```

---

### 28. **`sort()`**

* A **list method** that sorts in-place (modifies original list).
* Optional `key=` and `reverse=`.

```python
nums = [5, 2, 9]
nums.sort()
print(nums)  # [2, 5, 9]
```

---

### 29. **`sorted()`**

* A **built-in** function that returns a **new sorted list**.
* Doesn’t modify the original.

```python
nums = [5, 2, 9]
new_nums = sorted(nums)
print(nums)      # [5, 2, 9]
print(new_nums)  # [2, 5, 9]
```

---

### 30. **Slicing**

* Extracts parts of a list using `[start:stop:step]`.
* Default: start=0, stop=end, step=1.

```python
letters = ['a','b','c','d','e']
print(letters[1:4])    # ['b', 'c', 'd']
print(letters[::-1])   # reverse list
```

---

### 31. **List Unpacking**

* Split list into variables directly.

```python
a, b, c = [1, 2, 3]
x, *mid, y = [1, 2, 3, 4, 5]
# x=1, mid=[2,3,4], y=5
```

---

### 32. **Iterating**

* Use `for` loop or `enumerate()` to loop with index.

```python
for fruit in fruits:
    print(fruit)

for i, val in enumerate(fruits):
    print(i, val)
```

---

### 33. **Indexing**

* Access items with zero-based index.
* Negative indexing starts from end.

```python
nums = [10, 20, 30]
print(nums[0])   # 10
print(nums[-1])  # 30
```

---

### 34. **Iterables vs Iterators**

* **Iterable**: can be looped over (like list).
* **Iterator**: an object with `__next__()` and `__iter__()`.

```python
nums = [1, 2, 3]
it = iter(nums)
print(next(it))  # 1
print(next(it))  # 2
```

---

### 35. **`map()`**

* Applies a function to each item in an iterable.

```python
nums = [1, 2, 3]
squares = list(map(lambda x: x**2, nums))  # [1, 4, 9]
```

---

### 36. **`filter()`**

* Filters items based on a condition.

```python
nums = [1, 2, 3, 4]
evens = list(filter(lambda x: x % 2 == 0, nums))  # [2, 4]
```

---

### 37. **`reduce()`**

* Performs rolling computation to reduce items to a single value.
* From `functools`.

```python
from functools import reduce
nums = [1, 2, 3, 4]
total = reduce(lambda x, y: x + y, nums)  # 10
```

---

### 38. **List Comprehensions**

* Concise way to create lists with logic.

```python
# [expression for item in iterable if condition]
squares = [x**2 for x in range(5)]         # [0, 1, 4, 9, 16]
evens = [x for x in range(10) if x%2 == 0] # [0, 2, 4, 6, 8]
```

---

Here's a **detailed guide** for working with **🔑 Dictionaries** in Python:

---

### 39. **Dictionary**

* A **key-value** store: unordered, mutable, indexed by keys.
* Defined using `{key: value}` syntax.
* Keys must be **hashable** (immutable types like str, int, tuple), values can be anything.

```python
person = {
    "name": "Hari",
    "age": 30,
    "city": "Bangalore"
}

# Access
print(person["name"])     # Hari

# Add / Update
person["age"] = 31
person["country"] = "India"

# Remove
del person["city"]

# Methods
print(person.keys())      # dict_keys(['name', 'age', 'country'])
print(person.values())    # dict_values(['Hari', 31, 'India'])
print(person.items())     # dict_items([('name', 'Hari'), ...])

# Safe access
print(person.get("email", "Not found"))  # Default if key missing
```

---

### 40. **Dictionary Comprehension**

* Create dictionaries using concise syntax:
  `{key_expr: value_expr for item in iterable if condition}`

```python
# Example: square numbers 1–5
squares = {x: x**2 for x in range(1, 6)}  # {1:1, 2:4, ..., 5:25}

# Filtering example
even_squares = {x: x**2 for x in range(1, 6) if x % 2 == 0}
```

---

Here's a **detailed breakdown** of **🔢 Sets** in Python with quick examples:

---

### 41. **Set**

* **Unordered**, **mutable**, collection of **unique** elements.
* Defined with `{}` or `set()`.

```python
s = {1, 2, 3, 3}
print(s)  # {1, 2, 3}
s.add(4)
s.remove(2)
```

---

### 42. **Set Comprehension**

* Similar to list/dict comprehension but for sets.

```python
squares = {x**2 for x in range(5)}  # {0, 1, 4, 9, 16}
```

---

### 43. **Union (`|` or `set.union()`)**

* Combines all elements (no duplicates).

```python
a = {1, 2, 3}
b = {3, 4, 5}
print(a | b)           # {1, 2, 3, 4, 5}
```

---

### 44. **Intersection (`&` or `set.intersection()`)**

* Elements common to both sets.

```python
print(a & b)           # {3}
```

---

### 45. **Difference (`-` or `set.difference()`)**

* Elements in `a` not in `b`.

```python
print(a - b)           # {1, 2}
```

---

### 46. **Symmetric Difference (`^`)**

* Elements in either set, but not both.

```python
print(a ^ b)           # {1, 2, 4, 5}
```

---

### 47. **Subset (`<=`)**

* Check if all elements of `a` are in `b`.

```python
print({1, 2} <= a)     # True
```

---

### 48. **Superset (`>=`)**

* Check if `a` contains all elements of `b`.

```python
print(a >= {3})        # True
```

---

### 49. **Disjoint Sets (`isdisjoint()`)**

* True if no common elements.

```python
print(a.isdisjoint({7, 8}))  # True
```

---

Here's a clear and concise guide to **🛑 Exception Handling** in Python:

---

### 50. **`try…except`**

* Catches and handles exceptions to prevent crashes.

```python
try:
    x = 10 / 0
except ZeroDivisionError:
    print("Cannot divide by zero.")
```

---

### 51. **`try…except…finally`**

* `finally` always runs—used for cleanup (e.g., closing files).

```python
try:
    f = open("data.txt")
    data = f.read()
except FileNotFoundError:
    print("File not found.")
finally:
    print("Cleaning up...")
    f.close()
```

---

### 52. **`try…except…else`**

* `else` runs if no exception occurs—used to separate success logic.

```python
try:
    num = int("42")
except ValueError:
    print("Invalid input.")
else:
    print("Conversion succeeded.")
```

---

Here’s a precise guide to **🔂 More on Loops** in Python:

---

### 53. **`for…else`**

* `else` runs **only if loop wasn’t broken** via `break`.

```python
for n in range(5):
    if n == 10:
        break
else:
    print("Completed without break.")  # ✅ Will print
```

---

### 54. **`while…else`**

* `else` runs only if `while` exits **naturally** (no `break`).

```python
x = 0
while x < 3:
    print(x)
    x += 1
else:
    print("Loop ended normally.")
```

---

### 55. **`do…while` Loop Emulation**

* Python lacks `do…while`; simulate with `while True` + `break`.

```python
while True:
    user_input = input("Enter value: ")
    if user_input:
        break
```
Here's a concise, example-driven guide to **🧠 More on Functions** in Python:

---

### 56. **Unpacking Tuples**

* Function can return or accept multiple values (tuples) which can be unpacked.

```python
def get_point():
    return (3, 4)

x, y = get_point()   # Unpacks (3, 4)
```

---

### 57. **`*args`**

* Collects extra **positional arguments** as a tuple.

```python
def add_all(*args):
    return sum(args)

add_all(1, 2, 3)   # 6
```

---

### 58. **`**kwargs`**

* Collects extra **keyword arguments** as a dictionary.

```python
def greet(**kwargs):
    print(f"Hello {kwargs.get('name')} from {kwargs.get('city')}")

greet(name="Hari", city="Bangalore")
```

---

### 59. **Partial Functions**

* Fix arguments of a function using `functools.partial`.

```python
from functools import partial

def power(base, exp):
    return base ** exp

square = partial(power, exp=2)
square(4)   # 16
```

---

### 60. **Type Hints**

* Improves code readability and tooling; doesn’t enforce types at runtime.

```python
def greet(name: str, age: int) -> str:
    return f"{name} is {age} years old"
```

---

Here’s a clean breakdown of **📦 Modules & Packages** in Python:

---

### 61. **Modules**

* A **module** is any `.py` file that can contain variables, functions, classes.
* You import them using `import` or `from ... import`.

```python
# math_module.py
def add(x, y):
    return x + y

# main.py
from math_module import add
print(add(2, 3))
```

---

### 62. **Module Search Path**

* Python searches modules in this order:

  1. Current directory
  2. PYTHONPATH env var (if set)
  3. Standard lib directories (`sys.path`)

```python
import sys
print(sys.path)  # List of search directories
```

---

### 63. **`__name__` Variable**

* `__name__` is `"__main__"` when the file is **executed directly**.
* Used to write reusable code.

```python
def main():
    print("Run directly")

if __name__ == "__main__":
    main()
```

---

### 64. **Packages**

* A package is a **directory with `__init__.py`** and modules inside.
* Allows namespacing and modular design.

```
mypackage/
├── __init__.py
├── module1.py
└── module2.py
```

```python
from mypackage import module1
```

---

### 65. **Private Functions**

* Prefix with `_` to indicate **internal use only** (not enforced by Python).

```python
def _internal():
    print("Not for external use")
```

---

Here's a complete guide to **📁 Working with Files** in Python with simple and clear examples:

---

### 66. **Read Text File**

```python
with open("data.txt", "r") as f:
    content = f.read()
    print(content)
```

---

### 67. **Write Text File**

```python
with open("data.txt", "w") as f:
    f.write("Hello, World!")
```

---

### 68. **Create New File**

* Use `"x"` mode to **create** and raise an error if file exists.

```python
with open("new_file.txt", "x") as f:
    f.write("Created file.")
```

---

### 69. **Check File Existence**

```python
import os
print(os.path.exists("data.txt"))  # True or False
```

---

### 70. **Read CSV**

```python
import csv

with open("data.csv", newline='') as f:
    reader = csv.reader(f)
    for row in reader:
        print(row)
```

---

### 71. **Write CSV**

```python
import csv

data = [["name", "age"], ["Hari", 30]]
with open("data.csv", "w", newline='') as f:
    writer = csv.writer(f)
    writer.writerows(data)
```

---

### 72. **Rename File**

```python
import os
os.rename("data.txt", "renamed.txt")
```

---

### 73. **Delete File**

```python
import os
os.remove("data.txt")
```

---

Here’s a quick guide to **📂 Working with Directories** in Python:

---

### 74. **Directory Functions**

Use the `os` and `os.path` modules:

```python
import os

# Create a new directory
os.mkdir("new_folder")

# Create nested directories
os.makedirs("folder/subfolder")

# Remove a directory
os.rmdir("new_folder")              # Only if empty
os.removedirs("folder/subfolder")  # Removes nested if all empty

# Change current working directory
os.chdir("folder")

# Get current directory
print(os.getcwd())
```

---

### 75. **List Files in Directory**

Use `os.listdir()` or `os.scandir()` for more details.

```python
import os

files = os.listdir(".")  # Lists files/folders in current dir
print(files)

# With filtering
only_files = [f for f in os.listdir(".") if os.path.isfile(f)]
print(only_files)
```

Here’s a crisp explanation of **🔤 Strings** in Python with examples:

---

### 76. **f-Strings (Formatted Strings)**

* Introduced in Python 3.6 for cleaner string interpolation.
* Use `f"..."` and embed expressions inside `{}`.

```python
name = "Hari"
age = 30
print(f"My name is {name} and I'm {age} years old.")
```

---

### 77. **Raw Strings**

* Prefix with `r"..."` to **ignore escape sequences** (great for regex, file paths).

```python
path = r"C:\Users\Hari\new_folder"
print(path)  # Prints exactly with backslashes
```

---

### 78. **Backslash (`\`)**

* Used to **escape** characters inside strings or break long lines.

```python
print("He said, \"Hello\".")       # Escapes quotes
long_str = "This is a long string \
split across lines."              # Line continuation
```

---

Here’s a compact guide to **📦 pip, PyPI & Virtual Environments**:

---

### 79. **PyPI and `pip`**

* **PyPI (Python Package Index):** Public repo of Python packages.
* **`pip`:** Tool to install packages from PyPI.

```bash
pip install requests         # Install package
pip show requests            # Package info
pip list                     # Installed packages
pip uninstall requests       # Remove package
```

---

### 80. **Virtual Environments**

* Isolate dependencies per project using `venv`.

```bash
# Create env
python -m venv venv

# Activate
# Windows:
venv\Scripts\activate
# macOS/Linux:
source venv/bin/activate

# Deactivate
deactivate
```

---

### 81. **`pipenv` on Windows**

* Combines package management + virtual envs.
* Automatically creates/activates envs with `Pipfile`.

```bash
pip install pipenv

# Create & install
pipenv install requests

# Activate shell
pipenv shell

# Exit shell
exit
```

---

Here's a clear and practical guide to **🧱 Python OOP** (Object-Oriented Programming):

---

### 82. **Object-Oriented Concepts**

* **Class**: Blueprint for creating objects.
* **Object**: Instance of a class.
* OOP features: **Encapsulation**, **Abstraction**, **Inheritance**, **Polymorphism**.

---

### 83. **Classes & Objects**

```python
class Car:
    def drive(self):
        print("Driving...")

c = Car()       # Object created
c.drive()
```

---

### 84. **Class Variables**

* Shared across all instances.

```python
class Car:
    wheels = 4   # class variable

print(Car.wheels)  # 4
```

---

### 85. **Instance Methods**

* Take `self` as the first argument and operate on instance data.

```python
class Car:
    def start(self):
        print("Engine started")
```

---

### 86. **`__init__()`**

* Constructor method, runs on object creation.

```python
class Car:
    def __init__(self, brand):
        self.brand = brand

c = Car("Tesla")
```

---

### 87. **Instance Variables**

* Defined via `self`; unique per object.

```python
class Car:
    def __init__(self, color):
        self.color = color
```

---

### 88. **Private Attributes**

* Prefix with `_` or `__` (name mangling) to indicate “private”.

```python
class Car:
    def __init__(self):
        self.__engine = "V8"
```

---

### 89. **Class Attributes**

* Same as class variables (shared). Accessed via class or instance.

```python
class Car:
    wheels = 4

c = Car()
print(c.wheels)     # 4
```

---

### 90. **Static Methods**

* No `self`; acts like a regular function but in class scope. Use `@staticmethod`.

```python
class Car:
    @staticmethod
    def honk():
        print("Beep beep!")
```

---

Great! Here's the continuation of **🧱 Python OOP – Advanced Topics**:

---

### 91. **Inheritance**

* A class (child) inherits from another class (parent).
* Allows code reuse and extension.

```python
class Vehicle:
    def move(self):
        print("Moving")

class Car(Vehicle):
    def honk(self):
        print("Beep")

c = Car()
c.move()   # Inherited
c.honk()   # Own method
```

---

### 92. **`super()`**

* Calls a method from the **parent class**.

```python
class Vehicle:
    def __init__(self, brand):
        self.brand = brand

class Car(Vehicle):
    def __init__(self, brand, model):
        super().__init__(brand)
        self.model = model
```

---

### 93. **Method Overriding**

* Redefine a method from the parent in the child class.

```python
class Vehicle:
    def start(self):
        print("Starting vehicle")

class Car(Vehicle):
    def start(self):
        print("Starting car")   # Overrides parent
```

---

### 94. **Property Decorator (`@property`)**

* Creates **getter methods** for attributes with clean syntax.

```python
class Circle:
    def __init__(self, radius):
        self._radius = radius

    @property
    def area(self):
        return 3.14 * self._radius ** 2
```

---

### 95. **`__str__()` and `__repr__()`**

* Define how objects are printed.

```python
class Car:
    def __init__(self, brand):
        self.brand = brand

    def __str__(self):
        return f"Car brand: {self.brand}"
```

---

### 96. **Abstract Base Classes**

* Use `abc` module to define abstract methods in base classes.

```python
from abc import ABC, abstractmethod

class Animal(ABC):
    @abstractmethod
    def speak(self):
        pass
```

Here’s a focused guide on **`@property`** in Python, covering all 3 use-cases:

---

### 97. **`@property`**

* Turns a **method into a getter** so you can access it like an attribute.

```python
class Circle:
    def __init__(self, radius):
        self._radius = radius

    @property
    def area(self):
        return 3.14 * self._radius ** 2

c = Circle(5)
print(c.area)  # Access like a variable, not c.area()
```

---

### 98. **Read-only Property**

* Simply **don't define a setter** method.

```python
class User:
    def __init__(self, username):
        self._username = username

    @property
    def username(self):
        return self._username

u = User("hari")
u.username = "john"  # ❌ AttributeError: can't set attribute
```

---

### 99. **Delete Property**

* Use `@property.deleter` to allow deleting the property via `del`.

```python
class Car:
    def __init__(self, model):
        self._model = model

    @property
    def model(self):
        return self._model

    @model.deleter
    def model(self):
        print("Deleting model...")
        del self._model

c = Car("Tesla")
del c.model
```

---

Here’s a clean breakdown of **Inheritance and Advanced OOP** concepts in Python:

---

### 100. **Inheritance**

* A class can inherit methods/attributes from a parent class.

```python
class Animal:
    def speak(self):
        print("Animal speaks")

class Dog(Animal):
    def bark(self):
        print("Dog barks")

d = Dog()
d.speak()  # inherited
```

---

### 101. **Method Overriding**

* Child class redefines a method from the parent.

```python
class Animal:
    def speak(self):
        print("Animal")

class Dog(Animal):
    def speak(self):
        print("Dog")   # overrides Animal.speak
```

---

### 102. **`super()`**

* Calls the parent class’s method—used in overridden methods or `__init__`.

```python
class A:
    def greet(self):
        print("Hello from A")

class B(A):
    def greet(self):
        super().greet()
        print("Hello from B")
```

---

### 103. **`__slots__`**

* Restricts instance attributes, reduces memory by removing `__dict__`.

```python
class Point:
    __slots__ = ['x', 'y']

    def __init__(self, x, y):
        self.x = x
        self.y = y

p = Point(1, 2)
# p.z = 3  # ❌ AttributeError: 'Point' object has no attribute 'z'
```

---

### 104. **Abstract Classes**

* Base classes that define a contract using `@abstractmethod`.

```python
from abc import ABC, abstractmethod

class Shape(ABC):
    @abstractmethod
    def area(self):
        pass

class Square(Shape):
    def area(self):
        return 4 * 4
```

---

Here’s a compact and practical guide to **Enumeration in Python** using the `enum` module:

---

### 105. **Enum**

* Create named constant groups.

```python
from enum import Enum

class Status(Enum):
    PENDING = 1
    APPROVED = 2
    REJECTED = 3

print(Status.APPROVED)     # Status.APPROVED
print(Status.APPROVED.name)  # 'APPROVED'
```

---

### 106. **Enum Aliases & `@unique`**

* Prevent value duplication using `@unique`.

```python
from enum import Enum, unique

@unique
class Color(Enum):
    RED = 1
    GREEN = 2
    BLUE = 3
    # GREEN_ALIAS = 2  ❌ would raise ValueError if uncommented
```

---

### 107. **Enum Customization**

* Add methods or override `__str__` for better output.

```python
class Role(Enum):
    ADMIN = 1
    USER = 2

    def describe(self):
        return f"Role: {self.name}"

print(Role.ADMIN.describe())  # Role: ADMIN
```

---

### 108. **`auto()`**

* Automatically assigns incremental values.

```python
from enum import Enum, auto

class Direction(Enum):
    NORTH = auto()
    EAST = auto()
    SOUTH = auto()
    WEST = auto()

print(Direction.SOUTH.value)  # 3
```

---

Here's a quick and clear breakdown of the **SOLID Principles** in Python:

---

### 109. **SRP – Single Responsibility Principle**

* A class should have **one reason to change** (one responsibility).

```python
class Invoice:
    def calculate_total(self): ...
    
class InvoicePrinter:
    def print_invoice(self, invoice): ...
```

✅ `Invoice` handles logic; `InvoicePrinter` handles output.

---

### 110. **OCP – Open/Closed Principle**

* Classes should be **open for extension, closed for modification**.

```python
class Discount:
    def apply(self, total): return total

class PercentageDiscount(Discount):
    def apply(self, total): return total * 0.9
```

✅ Add new discount types without modifying the base.

---

### 111. **LSP – Liskov Substitution Principle**

* Subclasses should be replaceable for their parent without breaking behavior.

```python
class Bird:
    def fly(self): ...

class Sparrow(Bird):  # ✅ Valid

class Ostrich(Bird):  # ❌ Violates LSP if fly() is required
    def fly(self): raise NotImplementedError()
```

✅ Split base classes if needed to avoid violating expectations.

---

### 112. **ISP – Interface Segregation Principle**

* Clients shouldn't be forced to depend on **unused methods**.

```python
class Printer:
    def print(self): ...

class Scanner:
    def scan(self): ...

class AllInOne(Printer, Scanner): ...
```

✅ Break big interfaces into smaller ones.

---

### 113. **DIP – Dependency Inversion Principle**

* Depend on **abstractions**, not concrete implementations.

```python
class NotificationService:
    def __init__(self, sender):  # sender is an interface
        self.sender = sender

class EmailSender:
    def send(self, msg): print(f"Email: {msg}")

notif = NotificationService(EmailSender())
```

✅ Enables flexibility and testability via dependency injection.

---

Here’s a concise and complete guide to:

---

### 🔗 **Multiple Inheritance**

---

### 114. **Multiple Inheritance**

* A class inherits from **more than one parent**.

```python
class A:
    def greet(self): print("Hello from A")

class B:
    def greet(self): print("Hello from B")

class C(A, B): pass

c = C()
c.greet()  # Follows MRO (A first here)
```

---

### 115. **MRO – Method Resolution Order**

* Python uses **C3 linearization** to resolve method calls.
* Use `.mro()` or `__mro__` to inspect.

```python
print(C.__mro__)
```

---

### 116. **Mixin**

* A **reusable class** with focused behavior, used alongside a main class.
* Should not be used standalone.

```python
class LoggerMixin:
    def log(self, msg): print(f"[LOG] {msg}")

class Service(LoggerMixin):
    def run(self): self.log("Service running")

Service().run()
```

---

### 📜 **Descriptors**

---

### 117. **Descriptors**

* Control attribute access using special methods:

  * `__get__(self, obj, type)`
  * `__set__(self, obj, value)`
  * `__delete__(self, obj)`

```python
class Uppercase:
    def __get__(self, obj, objtype=None):
        return obj._name.upper()
    
    def __set__(self, obj, value):
        obj._name = value

class Person:
    name = Uppercase()

p = Person()
p.name = "hari"
print(p.name)  # "HARI"
```

---

### 118. **Data vs Non-Data Descriptors**

* **Data Descriptor**: implements `__get__` and `__set__` → higher priority.
* **Non-Data Descriptor**: only `__get__` → overridden by instance attribute.

```python
class NonData:
    def __get__(self, obj, type=None):
        return "non-data"

class Demo:
    x = NonData()

d = Demo()
d.x = "overridden"
print(d.x)  # "overridden" (non-data is bypassed)
```

---

Here’s a crisp guide to **🧠 Metaprogramming** in Python:

---

### 119. **`__new__()`**

* Called **before `__init__()`**, responsible for creating the object.

```python
class Custom:
    def __new__(cls, *args, **kwargs):
        print("Creating instance")
        return super().__new__(cls)
    
    def __init__(self):
        print("Initializing")

obj = Custom()
```

---

### 120. **`type` Class**

* Python’s metaclass — used to create classes dynamically.

```python
MyClass = type("MyClass", (object,), {"x": 5})
print(MyClass().x)  # 5
```

---

### 121. **Metaclass**

* A **class of a class** that controls how classes are created.

```python
class MyMeta(type):
    def __new__(cls, name, bases, attrs):
        attrs["created_by_meta"] = True
        return super().__new__(cls, name, bases, attrs)
```

---

### 122. **Metaclass Example**

```python
class MyMeta(type):
    def __new__(cls, name, bases, dct):
        dct['hello'] = lambda self: "Hi from meta"
        return super().__new__(cls, name, bases, dct)

class Greet(metaclass=MyMeta):
    pass

g = Greet()
print(g.hello())  # Hi from meta
```

---

### 123. **`@dataclass`**

* Auto-generates `__init__`, `__repr__`, `__eq__`, etc.

```python
from dataclasses import dataclass

@dataclass
class Book:
    title: str
    price: float

b = Book("Python", 499.0)
print(b)  # Book(title='Python', price=499.0)
```

---

Here’s a clean guide to **🛑 Exceptions in OOP** with examples:

---

### 124. **Raising Exceptions**

* Use `raise` to throw an exception manually.

```python
class Account:
    def withdraw(self, amount):
        if amount > 1000:
            raise ValueError("Amount exceeds limit")
```

---

### 125. **Raise from Cause**

* Chain exceptions using `raise ... from ...` to preserve the original error.

```python
try:
    int("abc")
except ValueError as e:
    raise RuntimeError("Conversion failed") from e
```

---

### 126. **Custom Exceptions**

* Create by subclassing `Exception`.

```python
class InsufficientFunds(Exception):
    def __init__(self, balance):
        super().__init__(f"Insufficient funds. Balance: {balance}")

# Usage
raise InsufficientFunds(100)
```

Here's a concise and practical guide to **⚙️ Python Concurrency**:

---

### 127. **Processes vs Threads**

* **Thread**: Shares memory space, lightweight, good for I/O-bound tasks.
* **Process**: Own memory, heavier, better for CPU-bound tasks (via `multiprocessing`).

---

### 128. **`threading` Module**

* Built-in module to run code in parallel threads.

```python
import threading

def task():
    print("Running in thread")

t = threading.Thread(target=task)
t.start()
t.join()
```

---

### 129. **Extending Thread**

* Subclass `threading.Thread` for custom behavior.

```python
class MyThread(threading.Thread):
    def run(self):
        print("Custom thread logic")

t = MyThread()
t.start()
```

---

### 130. **Returning from Thread**

* Use shared variables or `queue.Queue`.

```python
from queue import Queue

def task(q):
    q.put("result")

q = Queue()
t = threading.Thread(target=task, args=(q,))
t.start()
t.join()
print(q.get())  # result
```

---

### 131. **Multithreading Example**

```python
import threading

def greet(name):
    print(f"Hello {name}")

names = ["Hari", "John", "Sara"]
threads = [threading.Thread(target=greet, args=(n,)) for n in names]

for t in threads: t.start()
for t in threads: t.join()
```

---

### 132. **Daemon Threads**

* Dies when the main thread dies (used for background tasks).

```python
t = threading.Thread(target=task)
t.daemon = True
t.start()
```

---

### 133. **Thread Pools**

* Manage many threads efficiently using `concurrent.futures`.

```python
from concurrent.futures import ThreadPoolExecutor

def square(n): return n * n

with ThreadPoolExecutor(max_workers=3) as executor:
    results = executor.map(square, [1, 2, 3])
    print(list(results))  # [1, 4, 9]
```

---

Here’s a clear and practical guide to **🔐 Thread Synchronization** in Python:

---

### 134. **`Lock`**

* Prevents race conditions by allowing only one thread to access a block at a time.

```python
import threading

lock = threading.Lock()
counter = 0

def increment():
    global counter
    with lock:
        for _ in range(1000):
            counter += 1
```

---

### 135. **`Event`**

* Used for signaling between threads.

```python
event = threading.Event()

def waiter():
    print("Waiting...")
    event.wait()
    print("Event triggered!")

threading.Thread(target=waiter).start()
event.set()  # Unblocks the waiter
```

---

### 136. **Stop Thread (Graceful Way)**

* Use a flag (e.g., `Event`) to signal stop—Python doesn’t allow killing threads directly.

```python
stop_event = threading.Event()

def run():
    while not stop_event.is_set():
        print("Running...")

t = threading.Thread(target=run)
t.start()
stop_event.set()  # Stop thread
```

---

### 137. **`Semaphore`**

* Controls access to a limited resource (e.g., 2 threads at a time).

```python
sem = threading.Semaphore(2)

def task(n):
    with sem:
        print(f"Thread {n} working")
        time.sleep(1)

for i in range(4):
    threading.Thread(target=task, args=(i,)).start()
```

---

Here's a compact guide on **🔄 Sharing Data** and **⚙️ Multiprocessing** in Python:

---

### 138. **Thread-safe Queue**

* `queue.Queue` is **safe for multiple threads**.
* Used to pass data between threads without race conditions.

```python
import threading
from queue import Queue

q = Queue()

def worker():
    while not q.empty():
        item = q.get()
        print(f"Processing {item}")
        q.task_done()

for i in range(5):
    q.put(i)

for _ in range(2):
    threading.Thread(target=worker).start()

q.join()
```

---

### 139. **`multiprocessing` Module**

* Creates **separate processes** (not threads) → better for CPU-bound tasks.

```python
from multiprocessing import Process

def task(name):
    print(f"Hello from {name}")

p = Process(target=task, args=("Process-1",))
p.start()
p.join()
```

---

### 140. **Process Pool**

* Use `Pool` to manage multiple worker processes.

```python
from multiprocessing import Pool

def square(n): return n * n

with Pool(4) as pool:
    results = pool.map(square, [1, 2, 3, 4])
    print(results)  # [1, 4, 9, 16]
```

---

Here’s a focused guide on **🔄 Async I/O in Python** using `asyncio`:

---

### 141. **Event Loop**

* Core of asyncio; manages async task execution.

```python
import asyncio

loop = asyncio.get_event_loop()
loop.run_until_complete(asyncio.sleep(1))
```

---

### 142. **`async/await`**

* Use `async def` to define a coroutine; `await` pauses until result.

```python
async def greet():
    await asyncio.sleep(1)
    print("Hello")

asyncio.run(greet())
```

---

### 143. **Creating Tasks**

* Schedule coroutines to run concurrently using `asyncio.create_task()`.

```python
async def worker(n):
    await asyncio.sleep(n)
    print(f"Done {n}")

async def main():
    t1 = asyncio.create_task(worker(1))
    t2 = asyncio.create_task(worker(2))
    await t1
    await t2

asyncio.run(main())
```

---

### 144. **Canceling Tasks**

```python
async def task():
    try:
        await asyncio.sleep(5)
    except asyncio.CancelledError:
        print("Task was cancelled")

t = asyncio.create_task(task())
t.cancel()
```

---

### 145. **Timeout Cancellation**

```python
async def work():
    await asyncio.sleep(2)

try:
    await asyncio.wait_for(work(), timeout=1)
except asyncio.TimeoutError:
    print("Timeout!")
```

---

### 146. **`asyncio.wait()`**

* Run multiple tasks and wait for them to complete or timeout.

```python
tasks = [asyncio.create_task(worker(i)) for i in range(3)]
done, pending = await asyncio.wait(tasks)
```

---

### 147. **Future**

* Low-level placeholder for a result; usually not created manually.

```python
future = asyncio.Future()
future.set_result("Done")
print(await future)
```

---

### 148. **`asyncio.gather()`**

* Run multiple coroutines in parallel and wait for **all** to finish.

```python
results = await asyncio.gather(worker(1), worker(2))
```

---

Here’s a compact guide to **🧠 Advanced Python Concepts**:

---

### 149. **References**

* Variables are **references** (pointers) to objects in memory.
* Multiple variables can point to the same object.

```python
a = [1, 2]
b = a
b.append(3)
print(a)  # [1, 2, 3] — both refer to same list
```

---

### 150. **Garbage Collection**

* Python uses **reference counting + cyclic GC**.
* Unreferenced objects are automatically deleted.

```python
import gc
gc.collect()  # manually trigger GC
```

---

### 151. **Dynamic Typing**

* Variables are **not bound to a type**; types are checked at runtime.

```python
x = 10      # int
x = "Ten"   # now str — valid
```

---

### 152. **Mutable & Immutable**

* **Mutable**: `list`, `dict`, `set`
* **Immutable**: `int`, `str`, `tuple`, `frozenset`

```python
x = (1, 2)  # immutable tuple
x[0] = 5    # ❌ TypeError
```

---

### 153. **`is` Operator**

* Compares **object identity**, not equality (`==`).

```python
a = [1, 2]
b = a
c = [1, 2]
print(a is b)  # True
print(a is c)  # False
```

---

### 154. **`None`**

* Represents **absence of a value**; singleton object.

```python
x = None
if x is None:
    print("No value")
```

---

Here’s a precise guide to **📌 Variable Scope** in Python:

---

### 155. **Built-in, Local, Global**

* **Built-in**: Names like `len`, `print` (in `builtins` module).
* **Local**: Inside current function/block.
* **Global**: Defined at the top-level of a module.

```python
x = "global"

def func():
    x = "local"
    print(x)  # local

func()
print(x)      # global
```

To modify a global inside a function:

```python
def change():
    global x
    x = "changed globally"
```

---

### 156. **`nonlocal`**

* Used to modify a **variable from the nearest enclosing scope** (not global).

```python
def outer():
    x = "outer"

    def inner():
        nonlocal x
        x = "modified"
    
    inner()
    print(x)  # modified

outer()
```

---

Here’s a focused guide on **🔧 Closures & Decorators** in Python:

---

### 157. **Closures**

* A closure is a **function remembering variables from its enclosing scope**, even after that scope is gone.

```python
def outer(msg):
    def inner():
        print(msg)  # msg is closed over
    return inner

greet = outer("Hello")
greet()  # Hello
```

---

### 158. **Decorators**

* A function that **wraps another function** to extend its behavior.

```python
def decorator(func):
    def wrapper():
        print("Before")
        func()
        print("After")
    return wrapper

@decorator
def say_hi():
    print("Hi")

say_hi()
```

---

### 159. **Decorators with Arguments**

* Requires **an extra wrapper layer**.

```python
def repeat(n):
    def decorator(func):
        def wrapper(*args, **kwargs):
            for _ in range(n):
                func(*args, **kwargs)
        return wrapper
    return decorator

@repeat(3)
def greet():
    print("Hello")

greet()  # Prints 3 times
```

---

### 160. **Class Decorators**

* A class can also be decorated (e.g., for logging, validation).

```python
def debug(cls):
    class Wrapped(cls):
        def __init__(self, *args, **kwargs):
            print(f"Creating instance of {cls.__name__}")
            super().__init__(*args, **kwargs)
    return Wrapped

@debug
class Person:
    def __init__(self, name):
        self.name = name
```

---

### 161. **Monkey Patching**

* Dynamically modify or replace methods/attributes **at runtime**.

```python
class Dog:
    def speak(self):
        return "woof"

def new_speak(self):
    return "meow"

Dog.speak = new_speak
print(Dog().speak())  # meow
```

---

Here's a concise guide to **✅ `namedtuple`** in Python:

---

### 162. **`namedtuple`**

* A **lightweight, immutable class** for storing fields with names (from `collections`).
* Access by **attribute name** or **index**.

```python
from collections import namedtuple

Person = namedtuple("Person", ["name", "age"])
p = Person(name="Hari", age=30)

print(p.name)   # Hari
print(p[1])     # 30
```

**Features:**

* Readable `__repr__`
* Immutable (like a tuple)
* Memory-efficient

✅ Great for replacing small classes or returning structured data.

---

Here’s a clear and practical guide on **🔢 Sequence Types** in Python:

---

### 163. **Sequences**

* Ordered collections that support:

  * Indexing: `x[0]`
  * Slicing: `x[1:3]`
  * Iteration: `for i in x`
  * Membership: `in`, `not in`
* Examples: `list`, `tuple`, `str`, `range`, `bytes`

---

### 164. **Lists vs Tuples**

| Feature     | `list`       | `tuple`              |
| ----------- | ------------ | -------------------- |
| Mutability  | ✅ Mutable    | ❌ Immutable          |
| Syntax      | `[1, 2]`     | `(1, 2)`             |
| Performance | Slower       | Faster (less memory) |
| Use case    | Dynamic data | Fixed data           |

---

### 165. **Slicing**

* Extract part of a sequence: `seq[start:stop:step]`

```python
x = [0, 1, 2, 3, 4]
print(x[1:4])     # [1, 2, 3]
print(x[::-1])    # [4, 3, 2, 1, 0]
```

---

### 166. **Custom Sequence Type**

* Create by implementing `__getitem__` and `__len__`.

```python
class CountDown:
    def __init__(self, start):
        self.start = start

    def __getitem__(self, index):
        if index >= self.start:
            raise IndexError
        return self.start - index

    def __len__(self):
        return self.start

cd = CountDown(5)
print(cd[0])  # 5
print(list(cd))  # [5, 4, 3, 2, 1]
```

---

Here's a clear and concise guide on **🔁 Iterators & Iterables** in Python:

---

### 167. **Iterators**

* An **iterator** is an object that implements:

  * `__iter__()` → returns itself
  * `__next__()` → returns next item or raises `StopIteration`

```python
nums = iter([1, 2, 3])
print(next(nums))  # 1
print(next(nums))  # 2
```

---

### 168. **Iterators vs Iterables**

| Feature    | Iterable                    | Iterator                                   |
| ---------- | --------------------------- | ------------------------------------------ |
| Definition | Can be looped over          | Generates items one at a time              |
| Examples   | `list`, `str`, `tuple`      | result of `iter()` call                    |
| Methods    | Must implement `__iter__()` | Must implement `__iter__()` & `__next__()` |

```python
lst = [1, 2, 3]         # iterable
it = iter(lst)          # iterator
```

---

### 169. **`iter()`**

* Converts an **iterable into an iterator**.
* Also supports a 2-arg form: `iter(callable, sentinel)`

```python
s = "Hari"
it = iter(s)
print(next(it))  # 'H'
```

```python
# Example: read lines until "stop"
def get_input():
    return input()

for line in iter(get_input, "stop"):
    print(f"You typed: {line}")
```

---

Here's a clear and quick guide to **⚡ Generators** in Python:

---

### 170. **Generator Functions**

* Use `yield` to produce a sequence **one value at a time**.
* Memory-efficient and lazy evaluation.

```python
def count_up(n):
    i = 1
    while i <= n:
        yield i
        i += 1

for num in count_up(3):
    print(num)  # 1, 2, 3
```

---

### 171. **Generator Expressions**

* Concise generator version of a loop; similar to list comprehensions but uses `()` instead of `[]`.

```python
squares = (x*x for x in range(4))
print(next(squares))  # 0
print(list(squares))  # [1, 4, 9]
```

---

Here’s a detailed and clean guide for:

---

### 🧩 **Context Managers**

---

### 172. **Context Manager**

* Ensures proper setup and teardown (e.g., file I/O).
* Use `with` keyword. You can also define custom managers using `__enter__` / `__exit__`.

```python
with open("file.txt", "r") as f:
    data = f.read()
```

Custom context manager:

```python
class Demo:
    def __enter__(self): print("Start"); return self
    def __exit__(self, exc_type, exc_val, exc_tb): print("End")

with Demo(): pass
```

---

### 🔢 **Integer & Boolean**

---

### 173. **Integer Internals**

* Python's `int` is unbounded.
* Small integers (-5 to 256) are **interned** (cached for reuse).

```python
a = 256
b = 256
print(a is b)  # True (same object)
```

---

### 174. **Floor Division (`//`)**

* Divides and **rounds down** to the nearest integer.

```python
print(7 // 2)   # 3
print(-7 // 2)  # -4
```

---

### 175. **Modulo (`%`)**

* Returns **remainder**, sign matches the **divisor** in Python.

```python
print(7 % 2)    # 1
print(-7 % 2)   # 1
```

---

### 176. **`bool`**

* Subclass of `int`: `True == 1`, `False == 0`.

```python
print(isinstance(True, int))  # True
print(True + True)            # 2
```

---

### 177. **`and`**

* Returns first **falsy** value or last value.

```python
print(0 and 5)     # 0
print(3 and 5)     # 5
```

---

### 178. **`or`**

* Returns first **truthy** value or last value.

```python
print(0 or 5)      # 5
print(3 or 5)      # 3
```

---

### 🌊 **Float**

---

### 179. **Float Internals**

* Python uses **IEEE 754 double precision** (`64-bit`).

```python
x = 0.1 + 0.2
print(x)  # 0.30000000000000004 (precision issue)
```

---

### 180. **float to int**

* Use `int()` to **truncate** decimal part (no rounding).

```python
print(int(3.99))  # 3
```

---

### 181. **Rounding**

* Use `round(number, digits)`.

```python
print(round(3.14159, 2))  # 3.14
```

---

### 💯 **Decimal**

---

### 182. **`decimal` Module**

* For **precise decimal arithmetic** (e.g., financial apps).

```python
from decimal import Decimal, getcontext

getcontext().prec = 4
x = Decimal("1.2345") + Decimal("0.0006")
print(x)  # 1.235
```





