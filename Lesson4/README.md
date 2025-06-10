# Lesson 4: Conditional Logic & Input

## Learning Objectives

- Understand Python conditional statements: `if`, `elif`, `else`  
- Use comparison operators: `==`, `!=`, `<`, `>`, `<=`, `>=` 
- Use `input()` to capture user input  
- Understand Python block indentation and nesting  

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

### Basic `if` Statement
```python
age = int(input("Enter your age: "))
if age >= 18:
    print("You are an adult.")
```
- Syntax: `if <condition>:` then indented block

### `if ... else`
```python
a = 32
b = 33
if b > a:
  print("b is greater than a")
elif a == b:
  print("a and b are equal")
```

### `if ... elif ... else`
```python
score = int(input("Enter your score (0–100): "))
if score >= 90:
    print("A")
elif score >= 80:
    print("B")
elif score >= 70:
    print("C")
else:
    print("F")
```

### Comparison Operators 
| Operator | Meaning          | Example  |
| :------: | :--------------- | :------- |
|   `==`   | equal            | `x == y` |
|   `!=`   | not equal        | `x != y` |
|    `>`   | greater than     | `x > y`  |
|    `<`   | less than        | `x < y`  |
|   `>=`   | greater or equal | `x >= y` |
|   `<=`   | less or equal    | `x <= y` |


## Exit-Ticket and Work Session Tasks
>Submit your Exit Tickets via Canvas

## Task 1: Positive/Negative/Zero Checker

**Problem:**  
Ask the user for a number and tell them if it’s positive, zero, or negative.

1. **Input & Type**
    - What built-in function lets you ask the user for a value?
    - How can we make sure it's a number? 
2. **Branching Logic**  
    - How many different conditions must you check?
3. **Testing**  
    - How do you output a message once you know which branch you’re in?

## Task 2: Cat-Color Loop with Early Exit

**Problem:**  
Loop through a list of cat colors; if you see `"blue"` or `"black"`, react and then stop the loop.

1. **Loop Structure**    
   - How do you write a `for` loop to iterate over `cats = ["brown","white","blue","black"]`?
2. **Condition Checks**  
   - How will you compare the current `color` to the string `"blue"`?  
   - If it matches, use `break` to stop the loop immediately.
3. **Default Case & Testing**  
   - What do you do when the color isn’t `"blue"` or `"black"`?  
