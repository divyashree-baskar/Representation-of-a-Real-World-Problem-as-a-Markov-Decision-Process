# Representation-of-a-Real-World-Problem-as-a-Markov-Decision-Process


## Aim

To represent a real-world problem using a Markov Decision Process (MDP) by defining its states, actions, transition probabilities, rewards, and Python representation.


---

## Problem Statement

### Problem Description

A student wants to reach college on time. The student can be in different situations, such as waking up, getting ready, waiting for the bus, travelling to college, or reaching college.

The agent decides what action to take at each stage. Rewards are given for reaching college on time, while penalties are given for delays.

This problem can be represented using a Markov Decision Process.


---

## MDP Components

A Markov Decision Process is represented as:

**MDP = (S, A, P, R, γ)**

Where:

- **S:** Set of states
- **A:** Set of actions
- **P:** Transition probability function
- **R:** Reward function
- **γ:** Discount factor

---

## State Space


The state space contains five possible situations of the student.

S = {

- S1: Student is sleeping
- S2: Student is getting ready
- S3: Student is waiting for the bus
- S4: Student is travelling to college
- S5: Student has reached college
}



---

## Sample State

**S3: Student is waiting for the bus.**

In this state, the student waits for the bus to travel to college.



---

## Action Space

The possible actions available to the student are:

A = {

- A1: Wake up
- A2: Get ready quickly
- A3: Wait for the bus
- A4: Board the bus
- A5: Reach the classroom
}



---

## Sample Action

**A2: Get ready quickly.**

The student chooses this action to save time and avoid being late.


---

## Transition Probability

Transition probability describes the chance of moving from one state to another after taking an action.

For example:

- From S1 to S2 after waking up: Probability = 1.0
- From S2 to S3 after getting ready: Probability = 0.9
- From S3 to S4 after boarding the bus: Probability = 0.8
- From S4 to S5 after travelling: Probability = 0.9

These probabilities are assumed for this example.

General form:

**P(s′ | s, a)**

It represents the probability of reaching the next state after taking an action in the current state.


This means:

> Probability of reaching next state $s'$ after taking action $a$ in current state $s$.


---

## Reward Function

The reward function gives feedback for each action.

- Reaching college on time: +10
- Getting ready quickly: +5
- Waiting for the bus: -1
- Being delayed: -5

A positive reward encourages good decisions, while a negative reward discourages delays.

The reward function defines the feedback received by the agent after taking an action.

General form:

$$
R(s,a,s')
$$



---

## Graphical Representation

The MDP can be represented as the following sequence:

Sleeping → Getting Ready → Waiting for Bus → Travelling to College → Reached College

The transitions are associated with actions, probabilities, and rewards.

<img width="1024" height="1536" alt="image" src="https://github.com/user-attachments/assets/10a3bbb4-7982-48cc-b579-7311f085d80a" />


---

## Python Representation

Write your code here.

Use Python dictionaries to represent the MDP.


```python
# MDP Representation using Python
# print("Name:       ")
# print("Register Number:     ")

```
---
## Output

Write your Python output here.


---

## Result

Thus, the real-world problem of a student travelling to college was successfully represented as a Markov Decision Process using five states, actions, transition probabilities, a reward function, and Python dictionaries.



---

