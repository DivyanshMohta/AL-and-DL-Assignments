# Assignment 1: 8-Puzzle Problem :
 This assignment implements Depth First Search (DFS) and Breadth First Search (BFS) to solve the 8-puzzle problem.

## Problem Statement: The 8-puzzle problem is a sliding tile puzzle where the goal is to arrange the tiles in numerical order with one blank tile.

## Description: 
Given a 3×3 board with 8 tiles (each numbered from 1 to 8) and one empty space, the objective is to place the numbers to match the final configuration using the empty space. We can slide four adjacent tiles (left, right, above, and below) into the empty space.

![image](https://github.com/user-attachments/assets/23e458d8-8c1a-4910-ab2e-acefd47a7626)

## 1. 8 puzzle Problem using DFS (Brute-Force) :
### Approach:
1. Start from the root node.
2. Explore the leftmost child node recursively until you reach a leaf node or a goal state.
3. If a goal state is reached, return the solution.
4. If a leaf node is reached without finding a solution, backtrack to explore other branches.

## 2. 8 puzzle Problem using BFS (Brute-Force) :
### Approach:
1. Start from the root node.
2. Explore the leftmost child node recursively until you reach a leaf node or a goal state.
3. If a goal state is reached, return the solution.
4. If a leaf node is reached without finding a solution, backtrack to explore other branches.
