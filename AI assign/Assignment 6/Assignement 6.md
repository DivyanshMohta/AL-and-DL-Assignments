# Assignment 6: 8-Queens Problem
This assignment demonstrates basic search strategies applied to the 8-Queens problem.

## Problem Statement
The objective of the 8-Queens problem is to place 8 queens on a chessboard such that no two queens can attack each other.

## Description:
The eight queens problem is the problem of placing eight queens on an 8×8 chessboard such that none of them attack one another (no two are in the same row, column, or diagonal). 
More generally, the n queens problem places n queens on an n×n chessboard.

### Algorithm
Let's go through the steps below to understand how this algorithm of solving the 8 queens problem using backtracking works:
1. Traverse all the rows in one column at a time and try to place the queen in that position.
2.  After coming to a new square in the left column, traverse to its left horizontal direction to see if any queen is already placed in that row or not. 
If a queen is found, then move to other rows to search for a possible position for the queen.
3.  Like step 2, check the upper and lower left diagonals. We do not check the right side because it's impossible to find a queen on that side of the board yet.
4. If the process succeeds, i.e. a queen is not found, mark the position as '1' and move ahead.
5.  Recursively use the above-listed steps to reach the last column. Print the solution matrix if a queen is successfully placed in the last column.
6.  Backtrack to find other solutions after printing one possible solution.

Example: One possible solution to the 8 queens problem using backtracking is shown below. In the first row, the queen is at E8 square, so we have to make sure no queen is in column E and row 8 and also along its diagonals. 
Similarly, for the second row, the queen is on the B7 square, thus, we have to secure its horizontal, vertical, and diagonal squares. 
The same pattern is followed for the rest of the queens. 

![image](https://github.com/user-attachments/assets/fcfb67bf-1508-4420-95dc-e0272d9631a3)

Output:

 

0 0 0 0 1 0 0 0

0 1 0 0 0 0 0 0

0 0 0 1 0 0 0 0

0 0 0 0 0 0 1 0

0 0 1 0 0 0 0 0

0 0 0 0 0 0 0 1

0 0 0 0 0 1 0 0

1 0 0 0 0 0 0 0
