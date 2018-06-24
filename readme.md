# Lesson 1
## Why should you learn to code?
It is cool, and fun.

## Setup
Install:
1. Python version 3.6.x
2. Visual Studio Code


## Binary Code
All code eventually becomes a sequence of 0s and 1s that the processor executes.
Where the number system we use in every day life is base 10, binary code is simply base 2.

### Base 10

Number | Value
---|---
0|0
1|1
2|2
3|3
4|4
5|5
6|6
7|7
8|8
9|9
10|10
11|11

### Binary, base 2
Number | Value
---|---
0|0
1|1
10|2
11|3
100|4
101|5
110|6

## Types
When you write a progam, every piece of information you want to temporarily save has a type.

Type |Explanation| Example
---|---|---
Char| A single character, and no more| c
String|A sequence of characters|I am a string
Int|An integer value, essentially a whole number | 0, 1, 2
Float|A floating point number, a number with a decimal point|1.0, 2.232
Boolean|A true or false value|True, False

This list is not exhaustive, there are other types to know, but these are the most fundamental.

## Variables and Functions
Fortunately, in Python, you often don't need to explicitly state what type a variable is, Python will infer it for it.

Let's look at some variable declarations.

```python
number_variable = 1           # assigns the integer 1 to a variable called      "number_variable"
string_variable = "how r u?"  # assigns the string inside the "" to a variable
```

You can do cool things with variables, such as simple arithmetic.

```python
a = 1
b = 2

c = a + b   # c contains 1 + 2 = 3
d = a * b   # d contains 1 * 2 = 2
e = a / b   # e contains 1 / 2 = 0.5
```

## First Program
Let's write our first piece of code!

Create a file called "hello.py". In the file put:
```python
a = "Hello World!"
print(a)           # This print function outputs the value within the () to the terminal.
```
Next, open the terminal, navigate to the folder in which "hello.py" is stored, and type:
```
python hello.py
```

## Writing a function
A function is a piece of code that doesn't actually run until you explicitly call it, and ask it to run. A function can return a value back to whatever called the function.

Let's write a function that calculates the square of a number.

Create a file called "square.py" and add this:
```python
def square(num):        # This is our function declaration, called "square".
    return num * num

number = 12
number_squared = square(number)

print(number_squared)
```
Run this progam the same way we ran the progam in the previous section!

It's not very useful is it? It only calculates the square of 12. Let's add a modification.

```python
def square(num):
    return num * num

value = input("Enter a number: ")   # Asks for an input. Stores as String.
num = int(value)                    # Convert String to Integer

num_squared = square(num)           # Call function
print(num_squared)
```
Now we have a program that can square any number you want!

## Operators
You can use operators to test one value against another.
```python
1 == 1
1 == 2

1 < 2
1 < 1

1 <= 2
1 <= 1

True and True
True and False
False and False

True or True
True or False
False or False
```
Try these in the terminal. Activate the interpreter by typing "python" into the terminal. See if you can guess the results of the above commands.

## if statements
We can use if statements to execute a certain piece of code if something is true, and something else otherwise.
```python
if 1 == 1:
    print("True")
else:
    print("False")
```
Using if statements, let's write a function that determines whether a number is divible by 3.
```python
def is_divisible_by_3(num):
    if num % 3 == 0:
        return True
    else:
        return False

num = int(input("Enter a number: "))

if is_divisible_by_3(num):
    print("Yes!")
else
    print("No!")
```
Run this progam and see what happens. See if you can figure out what's happening in the code.

## Loops
A lot of the time, you need to repeat the same code a number of times. In this case, you would use a for loop.

We can write a function that prints every number up to 10:

```python
def print_numbers:
    for num in range(0,10):
        print(num)

print_numbers()
```

While loops are similar to for loops, but work slightly differently.
```python
count = 0
while count < 10:
    print(count)
    count += 1
```

Try using a for or while loop to write a function that calculates the factorial of a number.