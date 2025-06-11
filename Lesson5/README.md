# Lesson 5: Randomness & For-Loops

## Learning Objectives

- Import and use Python’s `random` module  
- Generate random floats (`random.random()`) 
- Select random elements (`random.choice()`) 
- Iterate over lists with `for` loops   

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

### 1. Importing the random Module
- Brings in Python’s built-in library of random-number functions so you can call things like random.random() or random.choice().
```python
import random
```

### 2. `for` loops Refresher
```python
names = ["Alice", "Bob", "Charlie"]
```
- How would I use a loop to print each of the names in `names`?

- In `for variable in ...:`, the `variable` name is defined on the fly by the loop itself—you don’t need to pre-declare it.

### 3. `random.random()`
- Returns a float in the range 0.0 and 1.0
```python
print(random.random())  # e.g. 0.374837...
```

### 4. `random.choice(seq)`
- Picks a single random element from a list.
```python
colors = ["red", "green", "blue"]
print(random.choice(colors))  # e.g. "green"
```

- how might we use our names list from above and pick a random name from it?

### 5. password puzzle 
```python
options = ['paper', 'pencil', 'computer', 'glasses', 'shirt', 'shoes']

correct_password = random.choice(options)

for word in options:
  if word == correct_password:
    print(word.capitalize())
  else:
    print(word)

password_guess = input('Choose the password from the list.')

if password_guess == correct_password:
  print('You got it!')
else:
  print('Capitalization is key! Try again! ' )
```
- who can walk us through this code? 
