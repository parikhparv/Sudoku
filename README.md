# 🧩 Sudoku Solver

A **Java-based Sudoku puzzle solver** that automatically finds a valid solution to any solvable 9×9 Sudoku grid. It uses **recursive backtracking**, an algorithmic approach that explores possible values for empty cells, checks constraints in real time, and backtracks whenever a conflict arises. The solver maintains efficient state tracking using boolean arrays for rows, columns, and subgrids—allowing rapid validation and constraint checking during recursion.

---

## 🔍 Overview

This program demonstrates algorithmic problem-solving and object-oriented design in Java.  
It takes an unsolved Sudoku grid as input and outputs the fully solved grid in a neatly formatted display.

The solver:
- Efficiently explores the search space using recursion  
- Validates each move based on Sudoku’s three core rules (row, column, subgrid)  
- Uses **boolean constraint arrays** to reduce redundant checks and speed up execution  

---

## ⚙️ Features

- Solves any valid **9×9 Sudoku puzzle**
- Implements **recursive backtracking** for systematic exploration  
- Dynamically detects **rule violations** (row, column, subgrid conflicts)  
- Reads puzzle configuration from an **external text file** (0 represents an empty cell)  
- Demonstrates **clean object-oriented design** and effective state management  
- Displays both **initial and solved** Sudoku grids in a clear, readable console format  

---

## 🧠 How It Works

1. **Input Handling:**  
   The program reads a text file containing the initial Sudoku grid.  
   - Each line contains 9 integers separated by spaces.  
   - `0` represents an empty cell.  

2. **Recursive Backtracking (solveRB):**  
   - The solver identifies the next empty cell.  
   - It attempts to place digits `1–9`, checking each against Sudoku rules.  
   - If a number fits, it recursively proceeds to the next empty cell.  
   - If no number fits, it **backtracks**—undoing the last move and trying another value.  

3. **Validation:**  
   Boolean arrays track which numbers are used in each row, column, and 3×3 subgrid for constant-time validation.

4. **Output:**  
   Once a valid configuration is found, recursion unwinds and the program prints both the **original puzzle** and the **solved grid** in a readable table format.







