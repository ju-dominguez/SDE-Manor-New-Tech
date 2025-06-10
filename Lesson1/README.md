# Lesson 1: Variables & Data Types

## Learning Objectives
- Recognize and declare Python variable types: str, int, float, bool
- Apply snake_case naming conventions
- Write single-line comments (#) and TODO: notes

## Icebreaker
- Prompt: “What’s your favorite breakfast? Share it in one sentence.”

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

### Data Types
```python
name      = "Taylor"  # str
year      = 2025      # int
price     = 9.99      # float
is_open   = True      # bool
```

### Naming Conventions
- Valid: `favorite_color`, `num_peppers`
- Invalid: `Num@Peps!`, `green-peppers`, `2nd_place`

## Exit Ticket & Work Session Tasks
>Submit your Exit Tickets via Canvas

### Work Session Task 1 
Model your favorite meal with four variables (one of each type) and print each ingredient.

### Work Session Task 2 
```python
card_num  = 52
card_type = "rare"
print(f"Tony has {card_num} {card_type} cards.")
```
