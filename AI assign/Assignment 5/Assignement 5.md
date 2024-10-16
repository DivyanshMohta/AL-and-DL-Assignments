# Assignment 5 : MinMax Algorithm
This assignment implements minmax algorithm for game playing.

# Problem Statement:
Implement MinMax Algorithm for game playing.

## Description:
Minimax is a kind of backtracking algorithm that is used in decision making and game theory to find the optimal move for a player, 
assuming that your opponent also plays optimally. It is widely used in two player turn-based games such as Tic-Tac-Toe, Backgammon, Mancala, Chess, etc.

### Example: 
Consider a game which has 4 final states and paths to reach final state are from root to 4 leaves of a perfect binary tree as shown below. Assume you are the
maximizing player and you get the first chance to move, i.e., you are at the root and your opponent at next level. Which move you would make as a 
maximizing player considering that your opponent also plays optimally?

![image](https://github.com/user-attachments/assets/34f45059-2811-44ef-af3d-abf416927a29)

Since this is a backtracking based algorithm, it tries all possible moves, then backtracks and makes a decision. 

Maximizer goes LEFT: It is now the minimizers turn. The minimizer now has a choice between 3 and 5. Being the minimizer it will definitely choose the least among both, that is 3
Maximizer goes RIGHT: It is now the minimizers turn. The minimizer now has a choice between 2 and 9. He will choose 2 as it is the least among the two values.
Being the maximizer you would choose the larger value that is 3. Hence the optimal move for the maximizer is to go LEFT and the optimal value is 3.

Now the game tree looks like below :

![image](https://github.com/user-attachments/assets/dd53e24f-3969-458d-884e-ad5d49ae7440)

The above tree shows two possible scores when maximizer makes left and right moves.
