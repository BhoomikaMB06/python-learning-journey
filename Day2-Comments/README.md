## Python Comments

### Introduction

**Comments** are notes written inside a Python program to explain what the code does. Comments are ignored by the Python interpreter, which means they do not affect the execution of the program.

Comments are very useful for making code **easier to understand, read, and maintain**. They are especially helpful when working on large programs or when sharing code with other developers.

### Why Do We Use Comments?

Comments can be used to:

* Explain what a particular part of the code does.
* Make programs easier to understand.
* Add notes or reminders for yourself.
* Temporarily prevent a line of code from executing.
* Help other programmers understand your code.

### Single-Line Comments

In Python, a single-line comment starts with the **`#` symbol**.

```python
# This is a comment
print("Hello, World!")
```

Python ignores everything written after `#` on that line.

### Comment After Code

A comment can also be written on the same line as the code.

```python
print("Hello, World!")  # Display a message
```

### Multi-Line Comments

Python does not have a special multi-line comment symbol. However, multiple single-line comments can be written using `#`.

```python
# This program demonstrates
# how comments work
# in Python

print("Learning Python")
```

### Example Program

```python
# Store the student's name
name = "Bhoomika"

# Display the name
print(name)
```

### Output

```text
Bhoomika
```

### Important Point

Comments are **not executed by Python**. They are written for humans to understand the program.

For example:

```python
# This line will not be executed
print("Hello, Python!")
```

