# 🔁 Python Loops

Loops allow us to execute a block of code multiple times. Python provides two main types of loops: `for` loops and `while` loops.

---

## 🔹 For Loop
Use `for` loops when you know ahead of time how many times you want to iterate.

### ✅ Basic Example
```python
name = "Abhishek"
for i in name:
    print(i, end=" ")
```

### 🔸 Print Numbers
```python
# Print 1 to 5
for i in range(1, 6):
    print(i)

# Print squares of numbers 1 to 10
for i in range(1, 11):
    print(f"{i} * {i} = {i*i}")
```

### 🔸 Iterating Through Lists
```python
colors = ["Red", "Green", "Blue", "Yellow"]
for color in colors:
    print(color)
```

### 🔸 Nested For Loops
```python
for color in colors:
    print(color)
    for letter in color:
        print(letter)
```

### 🔸 Range Function
```python
# range(stop)
for i in range(5):
    print(i)

# range(start, stop)
for i in range(3, 8):
    print(i)

# range(start, stop, step)
for i in range(1, 12, 2):
    print(i)

# Reverse loop
for i in range(5, 0, -1):
    print(i)
```

### 🔸 More For Loop Examples
```python
# Table of 7
for i in range(1, 11):
    print(f"7 * {i} = {7 * i}")

# Even numbers 2 to 20
for i in range(2, 21, 2):
    print(i)

# Countdown
for sec in range(10, 0, -1):
    print(f"Countdown: {sec}")
print("Blast off!!!")
```

---

## 🔹 While Loop
Use `while` loops when the number of iterations is not known beforehand.

### ✅ Basic Examples
```python
# While loop increasing
i = 0
while i < 3:
    print(i)
    i += 1

# While loop decreasing
count = 5
while count > 0:
    print(count)
    count -= 1
```

### 🔸 Else with While Loop
```python
x = 5
while x > 0:
    print(x)
    x -= 1
else:
    print("counter is 0")
```

### 🔸 User Input Example
```python
secret = 7
guess = 0
while guess != secret:
    guess = int(input("Guess the number: "))
    if guess != secret:
        print("Wrong! Try again.")
print("Correct guess!!!")
```

---

## 🔹 Loop Control Statements
Used to alter the flow of the loop.

### 🛑 break
Immediately exits the loop.
```python
for i in range(1, 10):
    if i == 5:
        print("Stopping at 5")
        break
    print(i)
```

### 🔄 continue
Skips the current iteration and proceeds to the next.
```python
for i in range(1, 6):
    if i == 3:
        continue
    print(i)
```

### 🔲 pass
Placeholder that does nothing. Used to write logic later.
```python
for i in range(5):
    if i == 2:
        pass
    print(i)
```

> 🧠 Loops are essential for performing repetitive tasks in a clean and efficient way!

---

# 📌 SOME EXTRA AND IMPORTANT INFORMATION

## 🔁 Emulating Do-While Loop in Python

Python doesn’t have a built-in `do-while` loop, but we can emulate it using a `while True` loop and a `break` statement.

### 🔹 Basic Syntax
```python
while True:
    # code runs at least once
    if not condition:
        break
```

### 🔺 Example: Password Checker
```python
while True:
    password = input("Enter the password:")
    if password == "python123":
        print("Access granted!!!")
        break
    else:
        print("Wrong password, Try again!!")
```

### 🔺 Example: Keep Adding Until 0 is Entered
```python
while True:
    num = int(input("Enter a number (0 to stop): "))
    if num == 0:
        print("Loop ended")
        break
    print(f"You entered: {num}")
```

> 📝 Use this technique when your code needs to run **at least once** before checking the condition.
