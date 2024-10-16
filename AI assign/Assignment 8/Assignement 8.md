# Assignment 8: Backward Chaining Algorithm
This assignment implements the Backward Chaining algorithm for reasoning and decision-making.

## Problem Statement
The Backward Chaining algorithm is used in inference, where the goal is to prove a given query by working backward through known rules and facts.

## Description: 
Backward chaining is a goal-driven inference technique. It starts with the goal and works backward to determine which facts must be true to achieve that goal. This method is ideal for situations where the goal is clearly defined, and the path to reach it needs to be established.

### How Backward Chaining Works
Start with a Goal: The inference engine begins with the goal or hypothesis it wants to prove.
Identify Rules: It looks for rules that could conclude the goal.
Check Conditions: For each rule, it checks if the conditions are met, which may involve proving additional sub-goals.
Recursive Process: This process is recursive, working backward through the rule set until the initial facts are reached or the goal is deemed unattainable.

![image](https://github.com/user-attachments/assets/eeea7a9e-d5f5-46ec-ab15-2b87b9ca8240)


Example of Backward Chaining
In a troubleshooting system for network issues:

Goal: Determine why the network is down.
Rule: If the router is malfunctioning, the network will be down.
The system starts with the goal (network down) and works backward to check if the router is malfunctioning, verifying the necessary conditions to confirm the hypothesis.

### Advantages of Backward Chaining
Goal-Oriented: It is efficient for goal-specific tasks as it only generates the facts needed to achieve the goal.
Resource Efficient: It typically requires less memory, as it focuses on specific goals rather than exploring all possible inferences.
Interactive: It is well-suited for interactive applications where the system needs to answer specific queries or solve particular problems.
Suitable for Diagnostic Systems: It is particularly effective in diagnostic systems where the goal is to determine the cause of a problem based on symptoms.

### Disadvantages of Backward Chaining
Complex Implementation: It can be more complex to implement, requiring sophisticated strategies to manage the recursive nature of the inference process.
Requires Known Goals: It requires predefined goals, which may not always be feasible in dynamic environments where the goals are not known in advance.
Inefficiency with Multiple Goals: If multiple goals need to be achieved, backward chaining may need to be repeated for each goal, potentially leading to inefficiencies.
Difficulty with Large Rule Sets: As the number of rules increases, managing the backward chaining process can become increasingly complex.

