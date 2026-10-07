# Python Operators

Operators are special symbols or keywords used to perform operations on values and variables in Python.

For example:

```python
a = 10
b = 5

print(a + b)
```
Types of Operators in Python

Python provides several types of operators:

1.Arithmetic Operators
2.Comparison Operators
3.Logical Operators
4.Bitwise Operators
5.Assignment Operators
6.Identity Operators
7.Membership Operators
8.Ternary Operator

1. Arithmetic Operators

Arithmetic operators are used to perform mathematical operations such as addition, subtraction, multiplication, division, and more.
| Operator | Description    |
| -------- | -------------- |
| `+`      | Addition       |
| `-`      | Subtraction    |
| `*`      | Multiplication |
| `/`      | Division       |
| `//`     | Floor Division |
| `%`      | Modulus        |
| `**`     | Exponentiation |

#Example:
```python
print("Addition:", a + b)
print("Subtraction:", a - b)
print("Multiplication:", a * b)
print("Division:", a / b)
print("Floor Division:", a // b)
print("Modulus:", a % b)
print("Exponentiation:", a ** b)
```
Output
Addition: 19
Subtraction: 11
Multiplication: 60
Division: 3.75
Floor Division: 3
Modulus: 3
Exponentiation: 50625

#Note:The / operator returns a floating-point result, while // performs floor division.

2. Comparison Operators

Comparison operators are used to compare two values. They return either True or False.

| Operator | Description              |
| -------- | ------------------------ |
| `>`      | Greater than             |
| `<`      | Less than                |
| `==`     | Equal to                 |
| `!=`     | Not equal to             |
| `>=`     | Greater than or equal to |
| `<=`     | Less than or equal to    |

Example:
```
a = 13
b = 33

print(a > b)
print(a < b)
print(a == b)
print(a != b)
print(a >= b)
print(a <= b)
```
Output:
False
True
False
True
False
True

3. Logical Operators

Logical operators are used to combine or modify conditions.

Python has three main logical operators:| Operator | Description                                      |
| -------- | ------------------------------------------------ |
| `and`    | Returns `True` if both conditions are true       |
| `or`     | Returns `True` if at least one condition is true |
| `not`    | Reverses the result                              |

Example
```
a = True
b = False

print(a and b)
print(a or b)
print(not a)
```
Output:

False
True
False

The general precedence of logical operators is:not → and → or

4. Bitwise Operators

Bitwise operators perform operations on the binary representation of integers.

The main bitwise operators are:
| Operator | Description |            |
| -------- | ----------- | ---------- |
| `&`      | Bitwise AND |            |
| `        | `           | Bitwise OR |
| `^`      | Bitwise XOR |            |
| `~`      | Bitwise NOT |            |
| `<<`     | Left Shift  |            |
| `>>`     | Right Shift |            |

Example
```
a = 10
b = 4

print("AND:", a & b)
print("OR:", a | b)
print("NOT:", ~a)
print("XOR:", a ^ b)
print("Right Shift:", a >> 2)
print("Left Shift:", a << 2)
```
Output:

AND: 0
OR: 14
NOT: -11
XOR: 14
Right Shift: 2
Left Shift: 40

5. Assignment Operators

Assignment operators are used to assign values to variables.
| Operator | Example   | Meaning                 |      |                       |
| -------- | --------- | ----------------------- | ---- | --------------------- |
| `=`      | `a = 10`  | Assign                  |      |                       |
| `+=`     | `a += 5`  | Add and assign          |      |                       |
| `-=`     | `a -= 5`  | Subtract and assign     |      |                       |
| `*=`     | `a *= 5`  | Multiply and assign     |      |                       |
| `/=`     | `a /= 5`  | Divide and assign       |      |                       |
| `//=`    | `a //= 5` | Floor divide and assign |      |                       |
| `%=`     | `a %= 5`  | Modulus and assign      |      |                       |
| `**=`    | `a **= 5` | Exponentiate and assign |      |                       |
| `&=`     | `a &= 5`  | Bitwise AND and assign  |      |                       |
| `        | =`        | `a                      | = 5` | Bitwise OR and assign |
| `^=`     | `a ^= 5`  | Bitwise XOR and assign  |      |                       |
| `<<=`    | `a <<= 2` | Left shift and assign   |      |                       |
| `>>=`    | `a >>= 2` | Right shift and assign  |      |                       |

Example:
```
a = 10

a += 5
print(a)

a -= 3
print(a)

a *= 2
print(a)

a //= 4
print(a)
```
Output:

15
12
24
6

6. Identity Operators

Identity operators are used to check whether two variables refer to the same object.

The two identity operators are:

is
is not

Example
```
a = 10
b = 20
c = a

print(a is c)
print(a is not b)
```
Output
True
True

is checks object identity, while == checks whether two values are equal.

For example:
```
a = [1, 2, 3]
b = [1, 2, 3]

print(a == b)
print(a is b)
```
Output
True
False

7. Membership Operators

Membership operators are used to check whether a value exists in a sequence such as a list, tuple, string, or set.

The two membership operators are:

in
not in

Example
```
x = 24
y = 20

my_list = [10, 20, 30, 40, 50]

if x not in my_list:
    print("x is NOT present in the list")
else:
    print("x is present in the list")

if y in my_list:
    print("y is present in the list")
else:
    print("y is NOT present in the list")
```

Output:

x is NOT present in the list
y is present in the list
8. Ternary Operator

The ternary operator is also called a conditional expression. It allows us to write a simple if-else condition in a single line.

Syntax
value_if_true if condition else value_if_false
Example:
```
a = 10
b = 20

minimum = a if a < b else b

print(minimum)
```
Output
10

9. Operator Precedence

Operator precedence determines which operation is performed first when an expression contains multiple operators.

For example:
```
expr = 10 + 20 * 30

print(expr)
```
Output
610

Multiplication is performed before addition:

20 * 30 = 600
10 + 600 = 610

Using parentheses can change the order:

expr = (10 + 20) * 30

print(expr)
Output
900
10. Operator Associativity

When an expression contains operators with the same precedence, associativity determines the order in which they are evaluated.

For example:
```
print(100 / 10 * 10)
print(5 - 2 + 3)
print(5 - (2 + 3))
print(2 ** 3 ** 2)
```
Output
100.0
6
0
512

Most arithmetic operators with the same precedence are evaluated from left to right. Exponentiation (**) is evaluated from right to left.

For example:
```
2 ** 3 ** 2
```
is evaluated as:
```
2 ** (3 ** 2)
```
which gives:

512
