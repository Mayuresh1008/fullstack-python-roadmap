# 🧭 Python Conditional Statements 

Conditional statements let you control the flow of your program by executing code blocks based on conditions.

## ✅ If Statement
Executes code if the condition is true.
```python
age = 18
if age >= 18:
    print("You can vote!")
```

## 🔁 If-Else Statement
Provides an alternative when the `if` condition is false.
```python
age = int(input("Enter your age: "))
if age >= 18:
    print("You can drive")
else:
    print("You cannot drive")
```

## ➕ Elif Statement
Checks multiple conditions sequentially.
```python
num = int(input("Enter a number:"))
if num < 0:
    print("Number is negative")
elif num > 0:
    print("Number is positive")
elif num >= 999:
    print("Number is Special and out of range")
else:
    print("Number is zero")
```

## 🧠 Nested If Statements
Using if statements within other if statements.
```python
num = 18
if num > 0:
    if num <= 10:
        print("Number is between 1-10")
    elif num <= 20:
        print("Number is between 11-20")
    else:
        print("Number is greater than 20")
```

## 🪜 One-Line Conditionals (Ternary Operator)
Compact way of writing simple if-else.
```python
age = 20
status = "Adult" if age >= 18 else "Minor"
print(status)
```

## 🔄 Boolean Logic in Conditions
Combining conditions with logical operators.
```python
if age >= 18 and has_id:
    print("Access granted")

if day == "Saturday" or day == "Sunday":
    print("It's the weekend!")

if not is_raining:
    print("No umbrella needed")
else:
    print("Take umbrella with you")
```

