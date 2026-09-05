# Python Tutorial

A beginner-friendly Python tutorial covering the fundamentals and commonly used concepts in real-world software development.

## Table of Contents

- [1. Introduction](#1-introduction)
- [2. Installation](#2-installation)
- [3. Hello World](#3-hello-world)
- [4. Variables](#4-variables)
- [5. Data Types](#5-data-types)
- [6. Operators](#6-operators)
- [7. Input and Output](#7-input-and-output)
- [8. Conditional Statements](#8-conditional-statements)
- [9. Loops](#9-loops)
- [10. Lists](#10-lists)
- [11. Tuples](#11-tuples)
- [12. Sets](#12-sets)
- [13. Dictionaries](#13-dictionaries)
- [14. Functions](#14-functions)
- [15. Lambda Functions](#15-lambda-functions)
- [16. Exception Handling](#16-exception-handling)
- [17. File Handling](#17-file-handling)
- [18. Modules and Packages](#18-modules-and-packages)
- [19. Object-Oriented Programming](#19-object-oriented-programming)
- [20. List Comprehension](#20-list-comprehension)
- [21. Virtual Environment](#21-virtual-environment)
- [22. Installing Packages with pip](#22-installing-packages-with-pip)
- [23. Mini Project](#23-mini-project)
- [24. Practice Exercises](#24-practice-exercises)

---

## 1. Introduction

Python is a popular programming language known for its simple and readable syntax. It is widely used in many fields, including:

- Web Development
- Data Science
- Machine Learning
- Artificial Intelligence
- Automation
- Backend Development
- API Development
- Data Engineering

Example:

```python
print("Hello, Python!")
```

---

## 2. Installation

Download Python from the official website:

https://www.python.org/

Check the installed Python version:

```bash
python --version
```

or:

```bash
python3 --version
```

Open the Python interpreter:

```bash
python
```

Exit the interpreter:

```python
exit()
```

---

## 3. Hello World

Create a file named:

```text
main.py
```

Add the following code:

```python
print("Hello, World!")
```

Run the program:

```bash
python main.py
```

---

## 4. Variables

Variables are used to store data.

```python
name = "Alice"
age = 25
height = 165.5
is_student = True

print(name)
print(age)
print(height)
print(is_student)
```

Python does not require you to declare the data type of a variable in advance.

```python
x = 10
x = "Hello"
```

---

## 5. Data Types

Common built-in data types in Python:

```python
name = "John"        # str
age = 30             # int
price = 99.99        # float
is_active = True     # bool
data = None          # NoneType
```

Check the data type of a variable:

```python
print(type(name))
print(type(age))
```

### Type Conversion

```python
age = "20"

age_number = int(age)

print(age_number + 5)
```

Other examples:

```python
x = int("10")
y = float("10.5")
z = str(100)
```

---

## 6. Operators

### Arithmetic Operators

```python
a = 10
b = 3

print(a + b)
print(a - b)
print(a * b)
print(a / b)
print(a // b)
print(a % b)
print(a ** b)
```

### Comparison Operators

```python
print(10 == 10)
print(10 != 5)
print(10 > 5)
print(10 < 5)
print(10 >= 10)
print(10 <= 20)
```

### Logical Operators

```python
age = 25

print(age >= 18 and age <= 60)
print(age < 18 or age > 60)
print(not age == 25)
```

---

## 7. Input and Output

Use `input()` to receive input from the user.

```python
name = input("Enter your name: ")

print("Hello", name)
```

Reading numeric input:

```python
age = int(input("Enter your age: "))

print(age + 1)
```

### f-string

```python
name = "Alice"
age = 25

print(f"My name is {name} and I am {age} years old.")
```

---

## 8. Conditional Statements

Use `if`, `elif`, and `else` to control program flow.

```python
score = 80

if score >= 80:
    print("Grade A")
elif score >= 70:
    print("Grade B")
elif score >= 60:
    print("Grade C")
else:
    print("Grade F")
```

Python uses indentation to define blocks of code.

```python
age = 20

if age >= 18:
    print("Adult")
```

---

## 9. Loops

### for Loop

```python
for i in range(5):
    print(i)
```

Output:

```text
0
1
2
3
4
```

Specify a range:

```python
for i in range(1, 6):
    print(i)
```

### while Loop

```python
count = 1

while count <= 5:
    print(count)
    count += 1
```

### break

Use `break` to stop a loop.

```python
for i in range(10):
    if i == 5:
        break

    print(i)
```

### continue

Use `continue` to skip the current iteration.

```python
for i in range(5):
    if i == 2:
        continue

    print(i)
```

---

## 10. Lists

A list stores multiple values in a single variable.

```python
fruits = ["apple", "banana", "orange"]

print(fruits)
```

Access list items:

```python
print(fruits[0])
print(fruits[1])
```

Add an item:

```python
fruits.append("mango")
```

Update an item:

```python
fruits[0] = "grape"
```

Remove an item:

```python
fruits.remove("banana")
```

Loop through a list:

```python
for fruit in fruits:
    print(fruit)
```

---

## 11. Tuples

A tuple is similar to a list, but its values cannot be changed after creation.

```python
point = (10, 20)

print(point[0])
print(point[1])
```

Tuples are useful for values that should remain unchanged.

```python
rgb = (255, 100, 50)
```

---

## 12. Sets

A set stores unique values.

```python
numbers = {1, 2, 3, 3, 4}

print(numbers)
```

The duplicate value `3` will only appear once.

Add an item:

```python
numbers.add(5)
```

Remove an item:

```python
numbers.remove(2)
```

---

## 13. Dictionaries

A dictionary stores data as key-value pairs.

```python
user = {
    "name": "Alice",
    "age": 25,
    "email": "alice@example.com"
}
```

Access values:

```python
print(user["name"])
print(user["age"])
```

Add or update values:

```python
user["age"] = 26
user["country"] = "Thailand"
```

Loop through a dictionary:

```python
for key, value in user.items():
    print(key, value)
```

---

## 14. Functions

Functions allow you to reuse blocks of code.

```python
def say_hello():
    print("Hello")
```

Call the function:

```python
say_hello()
```

### Function Parameters

```python
def greet(name):
    print(f"Hello, {name}")
```

```python
greet("Alice")
greet("Bob")
```

### Return Value

```python
def add(a, b):
    return a + b


result = add(10, 20)

print(result)
```

### Default Parameters

```python
def greet(name="Guest"):
    print(f"Hello, {name}")


greet()
greet("Alice")
```

---

## 15. Lambda Functions

A lambda function is a small anonymous function.

```python
add = lambda a, b: a + b

print(add(10, 20))
```

Example with `map()`:

```python
numbers = [1, 2, 3, 4]

squared = list(map(lambda x: x ** 2, numbers))

print(squared)
```

---

## 16. Exception Handling

Use `try` and `except` to handle errors.

```python
try:
    number = int(input("Enter a number: "))
    result = 10 / number

    print(result)

except ValueError:
    print("Please enter a valid number.")

except ZeroDivisionError:
    print("Cannot divide by zero.")
```

Use `finally` for code that should always run:

```python
try:
    print("Running...")
finally:
    print("Finished")
```

---

## 17. File Handling

### Write to a File

```python
with open("example.txt", "w", encoding="utf-8") as file:
    file.write("Hello Python")
```

### Read a File

```python
with open("example.txt", "r", encoding="utf-8") as file:
    content = file.read()

print(content)
```

### Append to a File

```python
with open("example.txt", "a", encoding="utf-8") as file:
    file.write("\nNew line")
```

---

## 18. Modules and Packages

Create a file named:

```text
calculator.py
```

Add the following functions:

```python
def add(a, b):
    return a + b


def subtract(a, b):
    return a - b
```

Use the module in `main.py`:

```python
import calculator

print(calculator.add(10, 5))
```

Or import a specific function:

```python
from calculator import add

print(add(10, 5))
```

---

## 19. Object-Oriented Programming

### Classes and Objects

```python
class User:

    def __init__(self, name, age):
        self.name = name
        self.age = age

    def introduce(self):
        print(f"My name is {self.name}")
```

Create an object:

```python
user = User("Alice", 25)

print(user.name)

user.introduce()
```

### Inheritance

```python
class Animal:

    def speak(self):
        print("Animal sound")


class Dog(Animal):

    def speak(self):
        print("Woof!")
```

```python
dog = Dog()

dog.speak()
```

---

## 20. List Comprehension

List comprehensions provide a concise way to create lists.

Traditional approach:

```python
numbers = []

for i in range(1, 6):
    numbers.append(i * 2)

print(numbers)
```

Using list comprehension:

```python
numbers = [i * 2 for i in range(1, 6)]

print(numbers)
```

Add a condition:

```python
even_numbers = [i for i in range(10) if i % 2 == 0]

print(even_numbers)
```

---

## 21. Virtual Environment

A virtual environment isolates project dependencies.

Create a virtual environment:

```bash
python -m venv .venv
```

### Windows

```bash
.venv\Scripts\activate
```

### macOS / Linux

```bash
source .venv/bin/activate
```

Deactivate the environment:

```bash
deactivate
```

---

## 22. Installing Packages with pip

Install a package:

```bash
pip install requests
```

List installed packages:

```bash
pip list
```

Create a `requirements.txt` file:

```bash
pip freeze > requirements.txt
```

Install dependencies from `requirements.txt`:

```bash
pip install -r requirements.txt
```

Example using `requests`:

```python
import requests

response = requests.get("https://api.github.com")

print(response.status_code)
```

---

## 23. Mini Project

Build a simple Todo List application.

```python
todos = []


def show_menu():
    print("\nTodo List")
    print("1. Add Todo")
    print("2. Show Todos")
    print("3. Exit")


while True:
    show_menu()

    choice = input("Choose menu: ")

    if choice == "1":
        todo = input("Enter todo: ")
        todos.append(todo)

        print("Todo added.")

    elif choice == "2":
        if not todos:
            print("No todos.")
            continue

        for index, todo in enumerate(todos, start=1):
            print(f"{index}. {todo}")

    elif choice == "3":
        print("Goodbye!")
        break

    else:
        print("Invalid menu.")
```

---

## 24. Practice Exercises

Try solving the following exercises by yourself.

### Beginner

1. BMI Calculator
2. Even/Odd Number Checker
3. Grade Calculator
4. Multiplication Table Generator
5. Find the Maximum Value in a List

### Intermediate

1. Todo List
2. Contact Management System
3. Expense Tracker
4. Password Generator
5. Number Guessing Game

### Advanced

1. REST API with FastAPI
2. Web Scraping
3. CRUD Application
4. Authentication System
5. RAG Application
6. AI Chatbot
7. Agentic RAG

---

## Recommended Learning Path

A recommended learning sequence:

```text
Python Syntax
    ↓
Variables & Data Types
    ↓
Conditions
    ↓
Loops
    ↓
List / Dict / Set / Tuple
    ↓
Functions
    ↓
Exception Handling
    ↓
File Handling
    ↓
Modules & Packages
    ↓
OOP
    ↓
Virtual Environment
    ↓
Third-party Libraries
    ↓
Projects
```

After learning the Python fundamentals, you can choose a specialization based on your interests.

### Backend Development

```text
Python
→ FastAPI / Django
→ Database
→ REST API
→ Docker
```

### Data Science

```text
Python
→ NumPy
→ Pandas
→ Matplotlib
→ Jupyter
```

### AI / Machine Learning

```text
Python
→ NumPy
→ Pandas
→ Scikit-learn
→ PyTorch
→ Transformers
```

### Generative AI / RAG

```text
Python
→ API
→ LLM
→ Embeddings
→ Vector Database
→ RAG
→ Advanced RAG
→ Agentic RAG
```

---

## Useful Commands

```bash
python --version
python main.py
python -m venv .venv
pip install <package>
pip list
pip freeze > requirements.txt
pip install -r requirements.txt
```

---

## Summary

Important Python topics to understand:

- Variables
- Data Types
- Conditions
- Loops
- Lists
- Dictionaries
- Functions
- Exception Handling
- File Handling
- Modules
- OOP
- Virtual Environment
- pip
- Project Structure

One of the best ways to learn Python is:

> Learn → Code → Build → Debug → Repeat

Practice by writing code and building projects alongside learning the theory.
