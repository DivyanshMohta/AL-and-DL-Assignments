# Assignment 2: Constraint Satisfaction Problem
  This assignment focuses on implementing a Constraint Satisfaction Problem (CSP) solver.

## Problem Statement: 
The goal is to solve a problem using constraints to limit possible solutions. This is commonly used in scheduling, coloring maps, or solving puzzles.

## Description:
Constraint Satisfaction Problems (CSP) play a crucial role in artificial intelligence (AI) as they help solve various problems that require decision-making 
under certain constraints. CSPs represent a class of problems where the goal is to find a solution that satisfies a set of constraints.
Example :

![image](https://github.com/user-attachments/assets/04ccb815-6765-4416-a1d0-de22ebf6aa6b)


### Constraint Satisfaction Problems (CSPs) consist of:

1. **Variables**: The elements needing values (e.g., cells in a Sudoku puzzle).
2. **Domains**: Possible values each variable can take (e.g., numbers 1-9 in Sudoku).
3. **Constraints**: Rules that restrict variable values (e.g., no repeated numbers in rows, columns, or boxes in Sudoku).

## CSP Algorithms: 
## 1. Backtracking Algorithm:
The backtracking algorithm is a depth-first search method used to systematically explore possible solutions in CSPs. It operates by assigning values to variables and backtracks if any assignment violates a constraint.

### How it works:

1. The algorithm selects a variable and assigns it a value.
2. It recursively assigns values to subsequent variables.
3. If a conflict arises (i.e., a variable cannot be assigned a valid value), the algorithm backtracks to the previous variable and tries a different value.
4. The process continues until either a valid solution is found or all possibilities have been exhausted.

## . Forward-Checking Algorithm
The forward-checking algorithm is an enhancement of the backtracking algorithm that aims to reduce the search space by applying local consistency checks.

### How it works:

1. For each unassigned variable, the algorithm keeps track of remaining valid values.
2. Once a variable is assigned a value, local constraints are applied to neighboring variables, eliminating inconsistent values from their domains.
3. If a neighbor has no valid values left after forward-checking, the algorithm backtracks.

## 3. Constraint Propagation Algorithms
Constraint propagation algorithms further reduce the search space by enforcing local consistency across all variables.

### How it works:

1. Constraints are propagated between related variables.
2. Inconsistent values are eliminated from variable domains by leveraging information gained from other variables.
3. These algorithms refine the search space by making inferences, removing values that would lead to conflicts.


