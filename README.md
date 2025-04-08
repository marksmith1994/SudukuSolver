# Sudoku Solver

This project is a C# console application designed to solve Sudoku puzzles using various algorithms. It allows users to input their own puzzles or use a default one, solve them with a selected algorithm, and compare the performance of different solving strategies.

## Features

*   Solve Sudoku puzzles using multiple algorithms.
*   Input custom Sudoku boards or use a built-in default puzzle.
*   Compare the execution time of different algorithms on the same puzzle.
*   Clear console display of the initial and solved boards.

## Algorithms Implemented

The following Sudoku solving algorithms are included:

1.  **Backtracking:** A standard recursive algorithm that tries filling digits and backtracks when it hits a dead end.
2.  **Constraint Propagation:** Enhances backtracking by deducing values based on constraints before resorting to guessing.
3.  **Dancing Links (Algorithm X):** An efficient exact cover algorithm adapted for Sudoku.
4.  **Bubble Sort (by possibilities):** A custom approach that sorts empty cells based on the number of possible values they can take before backtracking.
5.  **Heuristic Search:** Uses heuristics (like minimum remaining values, degree heuristic) to guide the search process.
6.  **Brute Force:** A simple backtracking implementation (similar to Backtracking but may have slight implementation differences).

## Getting Started

### Prerequisites

*   .NET SDK (Version compatible with the project, likely .NET 6.0 or later)

### Running the Application

1.  Clone the repository:
    ```bash
    git clone <repository-url>
    cd SudokuSolver
    ```
2.  Build the project:
    ```bash
    dotnet build
    ```
3.  Run the application:
    ```bash
    dotnet run --project SudokuSolver
    ```

Follow the on-screen prompts to:
*   Choose between solving a single Sudoku or comparing algorithms.
*   Select the algorithm(s) to use.
*   Decide whether to use the default board or input a custom 9x9 board (using 0 for empty cells).

## Project Structure

*   `SudokuSolver/`: Contains the main console application logic (`Program.cs`).
*   `SudokuSolver/Algorithm/`: Contains the interface (`ISudokuSolver.cs`), base class (`BaseSolver.cs`), and implementations for each solving algorithm.
*   `.gitignore`: Specifies intentionally untracked files that Git should ignore.
*   `README.md`: This file.
*   `SudokuSolver.sln` / `SudokuSolver.csproj`: Solution and project files.
