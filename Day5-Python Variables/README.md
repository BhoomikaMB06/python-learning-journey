# Python Variables

Variables are used to store data that can be referenced and used during program execution. A variable is a name assigned to a value.

Python does not require us to explicitly declare the data type of a variable. Python automatically determines the type based on the value assigned to it.

## 1. Creating Variables

A variable is created by assigning a value using the `=` operator.

x = 5
name = "Alex"

print(x)
print(name)
Output
5
Alex

In this example, x stores the integer value 5, while name stores the string "Alex".

2. Rules for Naming Variables

Python variables should follow these naming rules:

A variable name can contain letters, numbers, and underscores (_).
A variable name cannot start with a number.
Variable names are case-sensitive.
Python keywords such as if, else, for, and class cannot be used as variable names.
Spaces and special characters such as - should not be used in variable names.
Valid Variable Names
age = 21
_colour = "lilac"
total_score = 90
Invalid Variable Names
1name = "Error"
class = 10
user-name = "Doe"

The first example starts with a number, class is a Python keyword, and user-name contains a hyphen.

3. Assigning Values to Variables

Variables are assigned values using the = operator.

x = 5
y = 3.14
z = "Hi"

print(x)
print(y)
print(z)
Output
5
3.14
Hi
4. Dynamic Typing

Python is a dynamically typed language. This means that we do not need to specify the type of a variable when creating it.

A variable can also be assigned a different type of value later.

x = 10
print(x)

x = "Python"
print(x)
Output
10
Python

The variable x first contains an integer and later contains a string.

5. Assigning the Same Value to Multiple Variables

The same value can be assigned to multiple variables in one statement.

a = b = c = 100

print(a, b, c)
Output
100 100 100
6. Assigning Different Values to Multiple Variables

Python also allows us to assign different values to multiple variables in a single statement.

x, y, z = 1, 2.5, "Python"

print(x, y, z)
Output
1 2.5 Python
7. Variable Reassignment

A variable can be assigned a new value during program execution.

x = 1
y = x

y = y + 1

print(x)
print(y)
Output
1
2

Initially, x and y contain the value 1. When y = y + 1 is executed, y becomes 2. The value of x remains 1.

8. Understanding Object References

Python variables reference objects rather than directly storing values in the way beginners often imagine.

For example:

x = 5
y = x

print(x)
print(y)

Both x and y refer to the value 5.

If we later change x:

x = "Geeks"

print(x)
print(y)
Output
Geeks
5

Changing x does not change y. The variable x now refers to a different object, while y still refers to 5.

9. Deleting a Variable

The del keyword can be used to delete a variable.

x = 10

del x

print(x)

After del x, the variable x no longer exists. Therefore, trying to access it produces a NameError.

Example Error
NameError: name 'x' is not defined
10. Practical Example: Swapping Variables

Python allows us to swap two variables without using a temporary variable.

a = 5
b = 10

a, b = b, a

print(a, b)
Output
10 5

The values of a and b are exchanged using multiple assignment.

11. Practical Example: Counting Characters

We can store the length of a string in a variable using the len() function.

word = "Python"

length = len(word)

print("Length of the word:", length)
Output
Length of the word: 6
