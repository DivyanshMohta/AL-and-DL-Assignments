# Assignment 7: Forward Chaining Algorithm
This assignment implements the Forward Chaining algorithm for reasoning and decision-making.

## Problem Statement
The Forward Chaining algorithm is used for inference and rule-based reasoning, applying rules to known facts to infer new facts.

## Description:
Forward chaining is a data-driven inference technique. It starts with the available data and applies rules to infer new data until a 
goal is reached. This method is commonly used in situations where the initial data set is extensive, and the goal is to derive conclusions from it.

### How Forward Chaining Works
Start with Known Facts: The inference engine begins with the known facts in the knowledge base.
Apply Rules: It looks for rules whose conditions are satisfied by the known facts.
Infer New Facts: When a rule is applied, new facts are inferred and added to the knowledge base.
Repeat: This process is repeated until no more rules can be applied or a specified goal is achieved.


![image](https://github.com/user-attachments/assets/182fa8f4-8268-47aa-89a2-991443b80095)


Example of Forward Chaining
Consider a medical diagnosis system where rules are used to diagnose diseases based on symptoms:

Fact: The patient has a fever.
Rule: If a patient has a fever and a rash, they might have measles.
Starting with the known fact (fever), the system checks for other symptoms (rash). If the patient also has a rash, the system infers the possibility of measles.

### Advantages of Forward Chaining
Simplicity: Forward chaining is straightforward and easy to implement.
Automatic Data Processing: It processes data as it arrives, making it suitable for dynamic environments where new data continuously becomes available.
Comprehensive: It explores all possible inferences, ensuring that all relevant conclusions are reached.
Efficiency in Certain Scenarios: It can be efficient when all possible inferences need to be made from a set of data.

### Disadvantages of Forward Chaining
Inefficiency in Goal-Oriented Tasks: It can be inefficient if only a specific goal needs to be achieved, as it may generate many irrelevant inferences.
Memory Intensive: It can consume significant memory, storing a large number of intermediate facts.
Complexity with Large Rule Sets: As the number of rules increases, the system may become slow due to the need to check many conditions.
