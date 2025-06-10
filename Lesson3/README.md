# Lesson 3: Functions & Lists

## Learning Objectives

- Define and call functions (`def …:`) with parameters
- Understand local vs. global scope
- Create lists and iterate with `for` loops

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

### Why Functions?
- Modularity, reuse, readability, and reduction of repetition

### Defining & Calling
```python
def greet(name):
    print(f"Hello, {name}!")

greet("Sam")
```

### List Creation & Iteration
```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
```

### Nested Loops
```python
bases = ["plain", "chocolate", "blueberry"]
toppings = ["berries", "whipped cream", "walnuts"]
pancake_stacks = []
for base in bases:
    for topping in toppings:
        pancake_stacks.append(f"{base} pancake with {topping}")
print(pancake_stacks)
```
- The problem is broken-down into two explicit steps:
   1. Looping through each combination (for base → for topping)
    2. Building a list via append()

## Exit-Ticket and Work Session Tasks
>Submit your Exit Tickets via Canvas

### Work Session Task 1 
```python
# deck.py
ranks = ["A", "2", "3", "4", "5", "6", "7", "8", "9", "10", "J", "Q", "K"]
suits = ["♠", "♥", "♦", "♣"]
card_deck = []
for r in ranks:
    for s in suits:
        card_deck.append(f"{r} of {s}")
print(card_deck)
```

### Work Session Task 2 
```python
# lottery.py
winner       = "Kieth"
lottery_nums = [2, 5, 6, 3]
print("The winning numbers are:")
for num in lottery_nums:
    print(num)
print(f"Congratulations, {winner}! You just won 20,000 dollars!")
```

### Work Session Task 3 
```python
# cart.py
cart_prices = []

def add_to_cart(price):
    cart_prices.append(price)

def calculate_total():
    print(f"Total cost: ${sum(cart_prices):.2f}")

# Example usage
add_to_cart(19.99)
add_to_cart(5.50)
add_to_cart(3.25)
calculate_total()
```
