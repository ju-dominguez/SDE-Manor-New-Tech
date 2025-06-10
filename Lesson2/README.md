# Lesson 2: Basic I/O & String Operations

## Learning Objectives

- Use `print()` and `input()` for console I/O

- Convert types (`str()`, `int()`) when concatenating

- Recognize function-call syntax and separators


## Icebreaker 

- Prompt: “In one sentence, share a fun fact about you.”
- What special character do we use to wrap strings in code?

## GitHub Setup
1. Ensure you’re on your personal branch:
   ```bash
   git checkout julie
   ```
2. Fetch the latest main:
   ```bash
   git fetch origin main
   ```
3. Merge into your branch:
   ```bash
   git merge origin/main
   ```
4. At the end of class, don't forget to push your updates:
   ```bash
   git push origin julie
   ```

## Core Concepts 

### print() vs. input() 
``` python
name = input("What's your name? ")
print("Hello, " + name)
```

### Type Conversion 
*Error example*
```python
number_of_cookies = 5
print("You ate " + number_of_cookies + " cookies.")
```
*Fix using `str()`*
```python
print("You ate " + str(number_of_cookies) + " cookies.")
```

### Naming & Separators

- Use underscores (`_`) in identifiers
- Invalid: hyphens (`-`), spaces, special characters

### Function Calls

- Parentheses `()` signal definition or invocation
```python
def coffee_price():
  coffee = 3.00
  cookie = 2.00
  subtotal = coffee + cookie
  return subtotal

print(coffee_price())
```

## Exit-Ticket and Work Session Tasks
>Submit your Exit Tickets via Canvas

### Work Session Task 1 
```python
def receipt():
    # define item prices
    # sum them
    # apply 6% tax
    # print total
```

### Work Session Task 2 
```python
pennies     = 8
nickels     = 3
quarters    = 12
total_coins = pennies + nickels + quarters
print(f"I have {total_coins} coins.")
```

