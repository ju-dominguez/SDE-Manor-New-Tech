# Lesson 2: Basic I/O & String Operations

## Learning Objectives

- Use print() and input() for console I/O

- Convert types (str(), int()) when concatenating

- Recognize function-call syntax and separators


## Icebreaker (10 min)

- Prompt: “In one sentence, share a fun fact about you.”

- What special character do we use to wrap strings in code?

## Github setup (10 min)

- Get added to the section repo
- Create a branch for yourself
- Navigating lesson folders

## Core Concepts (40 min)

### print() vs. input() 

- Demo:
``` python
name = input("What's your name? ")
print("Hello, " + name)
```
- Explain prompting vs. output functions

### Type Conversion 

- Why `print("You ate " + number)` errors when `number` is int

- Demo `str(number_of_cookies)` inside concatenation

### Naming & Separators

- Underscores in identifiers; cannot use hyphens or spaces

### Function Calls

- Parentheses `()` signal call or definition

- Identify calls vs. definitions

- Demo:
```python
def coffee_price():
  coffee = 3.00
  cookie = 2.00
  subtotal = coffee + cookie

  return subtotal
```

### Exit-Ticket Time and Work Session Questions (30 min)

