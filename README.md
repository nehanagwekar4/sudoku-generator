# Sudoku Generator using Backtracking

A Python-based Sudoku puzzle generator built completely from scratch using the Backtracking algorithm.

Unlike a Sudoku solver, this project first generates a valid completed Sudoku board and then removes numbers while ensuring the puzzle still has a unique solution.

---

## Features

- Generates random Sudoku puzzles
- Three difficulty levels
  - Easy
  - Medium
  - Hard
- Uses recursive backtracking
- Ensures every generated puzzle has a unique solution
- Prints both the generated puzzle and its solution

---

## Algorithm

### Step 1
Generate a fully solved Sudoku board using recursive backtracking.

### Step 2
Randomly remove cells.

### Step 3
After removing each cell, verify that the puzzle still has exactly one solution.

If multiple solutions exist, restore the removed cell.

Repeat until the desired difficulty is reached.

---

## Difficulty Levels

| Difficulty | Empty Cells |
|------------|------------:|
| Easy | 35 |
| Medium | 45 |
| Hard | 53 |

> **Note:** Hard mode is configured with **53 empty cells** instead of 55 because the generator verifies puzzle uniqueness after every removal using recursive backtracking. Increasing the number of empty cells significantly increases generation time.

---

## Project Structure

```
sudoku_generator.py
```

Contains:

- Board generation
- Sudoku validation
- Recursive backtracking
- Solution counting
- Difficulty generation

---

## Concepts Used

- Recursion
- Backtracking
- Constraint Checking
- Randomization
- Matrix Manipulation
- Search Algorithms

---

## Future Improvements

- Faster uniqueness checking
- GUI using Tkinter or Pygame
- Web version using Streamlit
- PDF/Image puzzle export
- Difficulty based on solving techniques rather than clue count
