# 📘 Python Functions

Functions are reusable blocks of code designed to perform a specific task. They help make your code modular, cleaner, and more organized.

---

## ✅ What Are Functions?
A function is a reusable block of code that performs a task.

### 🔹 Types of Functions:
1. Built-in Functions (e.g., `print()`, `input()`, `len()`)
2. User-defined Functions (created using `def` keyword)

### 🔹 Function Syntax:
```python
def function_name(parameters):
    # code block
    return value
```

---

## 🔄 Using Functions

### 🔸 Example: Calculating Geometric Mean
```python
def calculateGmean(a, b):
    mean = (a * b) / (a + b)
    print(mean)

calculateGmean(9, 8)
```

### 🔸 Example: Checking Greater Number
```python
def isGreater(a, b):
    if a > b:
        print("First number is greater")
    else:
        print("Second number is greater or both are equal")

isGreater(9, 7)
```

---

## 🔣 Function Arguments and Return Types

### 🔹 Positional Arguments
```python
def average(a, b, c):
    print("The average is", (a + b + c)/3)

average(5, 6, 7)
```

## 🔣 Function Arguments and Return Types

### 🔹 Positional Arguments
```python
def average(a, b, c):
    print("The average is", (a + b + c)/3)

average(5, 6, 7)
```

### 🔹 Default Arguments
```python
def greet(name="Guest"):
    print(f"Hello, {name}!")

greet()
greet("Mayuresh")
```

### 🔹 Keyword Arguments
```python
def fullname(fname, mname, lname):
    print("Hello,", fname, mname, lname)

fullname(mname="Umesh", lname="Patil", fname="Mayuresh")
```

### 🔹 Required Arguments
```python
def average(a, b, c):
    print("The average is", (a + b + c)/3)

average(5, 6, 1)
```


### 🔹 Variable Length Positional Arguments (*args)
```python
def add_numbers(*numbers):
    total = 0
    for num in numbers:
        total += num
    print("Sum is:", total)

add_numbers(1, 2, 3, 4, 5)
```

### 🔹 Variable Length Keyword Arguments (**kwargs)
```python
def show_profile(**details):
    for key, value in details.items():
        print(f"{key}: {value}")

show_profile(name="Mayuresh", age=21, city="Vadodara")
```

---

## 🏁 Return Statement
```python
def average(*numbers):
    return sum(numbers) / len(numbers)

avg = average(5, 3, 6, 2)
print("Average of numbers:", avg)
```

---

## 🧪 4 Types of Functions:

### 1️⃣ No Parameters, No Return
```python
def say_hello():
    print("Hello!")

say_hello()
```

### 2️⃣ With Parameters, No Return
```python
def greet(name):
    print(f"Hi, {name}!")

greet("Mayuresh")
```

### 3️⃣ No Parameters, With Return
```python
def get_pi():
    return 3.14159

print(get_pi())
```

### 4️⃣ With Parameters and Return
```python
def add(a, b):
    return a + b

print("Sum:", add(10, 5))
```

---

## 🧰 Built-in Functions in Python
These come preloaded with Python:

### 🔹 Input/Output Functions
```python
print("Hello")
name = input("Enter your name: ")
```

### 🔹 Type Conversion
```python
print(int("10") + 5)
```

### 🔹 Type Checking
```python
x = 5.5
print(type(x))
print(isinstance(x, float))
```

### 🔹 Math Functions
```python
print(abs(-9))
print(round(3.14159, 2))
print(pow(2, 3))
```

### 🔹 Data Handling Functions
```python
fruits = ["apple", "banana"]
for index, fruit in enumerate(fruits):
    print(index, fruit)
```

### 🔹 Debug/Utility Functions
```python
print(id(10))
# help(str)
```

---

## 🧵 Example: All Argument Types Together
```python
def student_info(name, age=18, *hobbies, **details):
    print(name, age, hobbies, details)

student_info("Mayuresh", 20, "cricket", city="Vadodara", grade="A")
```

> 🚀 Functions are the foundation of reusable and scalable code in Python!
