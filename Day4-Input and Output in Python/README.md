Input and Output in Python

Input and output are important concepts in Python programming. Python provides the input() function to take information from the user and the print() function to display information on the screen.

The input() function is used to take input from the user. By default, the value returned by input() is a string. For example:

name = input("Enter your name: ")
print("Hello,", name, "! Welcome!")

Output:

Enter your name: GeeksforGeeks
Hello, GeeksforGeeks ! Welcome!

In this example, the user enters their name, the value is stored in the name variable, and the print() function displays a greeting message.

Printing Output Using print()

The print() function is used to display text, variables, and expressions on the screen. For example:

print("Hello, World!")

Output:

Hello, World!

We can also use the print() function to display variables. A single variable can be printed as follows:

name = "Brad"
print(name)

Output:

Brad

Multiple variables can also be printed by separating them with commas:

name = "Anjelina"
age = 25
city = "New York"

print(name, age, city)

Output:

Anjelina 25 New York
Taking Multiple Inputs

Python allows us to take multiple inputs from the user in a single line. The split() method can be used to separate the values entered by the user.

x, y = input("Enter two numbers: ").split()
print(x, y)

Output:

Enter two numbers: 10 20
10 20

The split() method separates the input values based on spaces. The values are stored in the variables x and y.

Taking Different Types of User Input

By default, the input() function returns a string. We can convert the input into other data types using type casting. Common types include int for integers and float for decimal numbers.

age = int(input("How old are you?: "))
number = float(input("Enter a decimal number: "))

print(age, number)

Output:

How old are you?: 23
Enter a decimal number: 3.5
23 3.5

In this example, int() converts the user's input into an integer, while float() converts the input into a decimal number.

We can also use input values to perform calculations. For example:

x = int(input("Enter first number: "))
y = int(input("Enter second number: "))

sum = x + y

print("Sum =", sum)

Output:

Enter first number: 10
Enter second number: 20
Sum = 30
