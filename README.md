# Sudoku
# Overview
A Java-based Sudoku puzzle solver that automatically finds a valid solution to any solvable 9×9 Sudoku grid. It uses recursive backtracking, an algorithmic approach that tries possible values in empty cells, checks constraints, and backtracks when conflicts arise. The solver efficiently tracks used numbers using boolean arrays for rows, columns, and subgrids, allowing rapid constraint checking during recursion.

# Features
• Solves any valid 9×9 Sudoku puzzle<br>
• Uses recursive backtracking for efficient exploration<br>
• Detects rule violations dynamically<br>
• Reads puzzle configuration from a text file<br>
• Demonstrates clean object-oriented design and state management<br>
• Displays both the initial and solved Sudoku grids in a readable format for user<br>

# How It Works
1. The program reads a text file containing the initial Sudoku grid (0 represents an empty cell)<br>
2. Each recursive call (solveRB) fills one cell of the grid, checking that the number does not violate Sudoku rules<br>
3. If a valid configuration is found, the recursion unwinds with a complete solution<br>
4. If a dead end is reached, the algorithm backtracks by removing the last value and trying the next one<br>






