---
layout: post
title: "How to Build a Calculator in Python"
date: 2026-03-01
categories: [learning, python]
---

## What I Learned

Today I learned how to build a simple calculator in Python. A calculator takes two numbers from the user and performs basic math operations like addition, subtraction, multiplication, and division.

## Key Points

- Use `input()` to get numbers from the user
- Use `if/elif/else` to choose which operation to do
- Always convert input to a number using `float()` or `int()`
- Handle division by zero so the program doesn't crash

## The Code

```python
def calculator():
    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))
    operation = input("Choose operation (+, -, *, /): ")

    if operation == "+":
        print("Result:", num1 + num2)
    elif operation == "-":
        print("Result:", num1 - num2)
    elif operation == "*":
        print("Result:", num1 * num2)
    elif operation == "/":
        if num2 == 0:
            print("Error! Cannot divide by zero.")
        else:
            print("Result:", num1 / num2)
    else:
        print("Invalid operation!")

calculator()
```

## Screenshot

![calculator screenshot](../images/calculator-screenshot.png)

## Source

Where I learned this from: paste the website or video link here.

---

*Tags: python, calculator, beginner*
