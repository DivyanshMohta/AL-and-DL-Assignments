# Assignment 3: Parsing Family Tree using Knowledge Base
This assignment involves building a family tree and parsing it using a knowledge base.

## Problem Statement
Create a knowledge base representing family relationships and use it to answer queries about the family tree.

## Description:

### Prolog :
Prolog is a logic programming language. It has important role in artificial intelligence. Unlike many other programming languages, 
Prolog is intended primarily as a declarative programming language. In prolog, logic is expressed as relations (called as Facts and Rules).

### Key Features :
1. Unification : The basic idea is, can the given terms be made to represent the same structure.
2. Backtracking : When a task fails, prolog traces backwards and tries to satisfy previous task.
3. Recursion : Recursion is the basis for any search in program.

### Syntax of Prolog Family Tree
The prolog syntax for mother-sister relationship is given as below:

![image](https://github.com/user-attachments/assets/a306bada-536f-4249-8c9e-6f9fa75cbace)

Mother Relationship

![image](https://github.com/user-attachments/assets/32c58032-04dd-4c8c-bcfa-23274720daca)

Sister Relationship

mother(M,N): parent(M,N), female(M).
sister(M,N): parent(O,M), parent(O,N), female(M), M\= =N.
