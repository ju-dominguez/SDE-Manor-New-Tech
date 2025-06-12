# Lesson 6: While-Loops

## Learning Objectives
- Understand the difference between `for` loops and `while` loops  
- Write a `while` loop that repeats until a condition is met  
- Use `break` to exit a loop early  
- Count iterations and guard against infinite loops  

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

### 1. `for` vs. `while`
- `for` loops are best when you know how many iterations you need (e.g., iterating through a list).
- `while` loops run UNTIL a condition becomes false—UNTIL being the keyword.

### 2. Basic `while` syntax
```python
count = 0
while count < 5:
    print(count)
    count += 1
    print("next loop starts")
```
- Starts at `count = 0`
- Checks `count < 5` each time BEFORE running the loop body
- Increments `count` so eventually `count < 5` becomes false and the loop stops

### 3. Exiting early with `break`
- Python break statement brings control out of the loop
```python
while True:
    answer = input("Type 'quit' to stop: ")
    if answer == "quit":
        break
    print("You typed:", answer)
```

### 4. Limiting Attempts (Skipping a False `if`)
```python
attempts = 0
while attempts < 3:
    guess = input("Guess the word: ")
    if guess == "python":
        print("Correct!")
        break
    attempts += 1
else:
    print("Out of attempts!")
```
- The `if` check (`guess == "python"`) runs each iteration; if false, Python skips the `print` and `break` lines, then does `attempts += 1`.
- If the loop completes all 3 iterations without a `break`, the `else:` block runs.

5. Counting Iterations & Avoiding Infinite Loops
```python
n = 2
while n < 11:
    print(n)
    n += 3
```
- Iterations:
  - Start at `n=2`, then `n=5`, then `n=8`.
  - When `n` becomes `11`, the condition `n < 11` is false and the loop stops.

- Total iterations: ?
