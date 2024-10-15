# Assignment 4: A* Algorithm
This assignment implements the A* algorithm for solving a specific application problem.

## Problem Statement
The A* algorithm is used to find the shortest path in a weighted graph. This assignment demonstrates its use in solving pathfinding problems.

## Description:
A* Search algorithm is one of the best and popular technique used in path-finding and graph traversals.
To approximate the shortest path in real-life situations, like- in maps, games where there can be many hindrances.
We can consider a 2D Grid having several obstacles and we start from a source cell (colored red below) to reach towards a goal cell (colored green below)

![image](https://github.com/user-attachments/assets/ad1e96f8-7ba6-498b-9ebf-39a87d1ef804)

In A* Search, the total cost \( f(n) = g(n) + h(n) \) combines the actual cost to reach a cell \( g(n) \) and the estimated cost to the goal \( h(n) \). To calculate \( h(n) \), we can either:

### A) **Exact Heuristics** (time-consuming)
1. Precompute distances between all cell pairs.
2. Use the Euclidean distance formula if there are no obstacles.

### B) **Approximation Heuristics** (faster)
1. **Manhattan Distance**: Sum of absolute differences in x and y coordinates. Use when moving in 4 directions.

![image](https://github.com/user-attachments/assets/b34eac55-92c3-4eac-8160-b27bb01dce56)


2. **Diagonal Distance**: Maximum of the absolute differences in x and y. Use when moving in 8 directions (like a chess King).

![image](https://github.com/user-attachments/assets/6a953fc7-0612-4756-b5c5-d36a0b7e699e)


3. **Euclidean Distance**: Straight-line distance between cells. Use when moving in any direction.

![image](https://github.com/user-attachments/assets/5a8b88e9-60fa-4cc6-94cb-6d1d5662a014)
