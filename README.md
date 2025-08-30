# MDP REPRESENTATION

## AIM:
To represent any one real-world problem in MDP form.

## PROBLEM STATEMENT:
To develop an environment in which a person is cycling top hill. The goal is to reach the top of the hill.

### Problem Description
The agent has to reach the goal state(top of hill) by taking the correct route towards the goal without drifting away from the path. After reaching the goal the agent will be rewarded if not then no reward will be provided.

### State Space
{0,1,2}

### Sample State
0->Hole State(bottom of the hill) 1->starting state(cycling starts) 2->Goal state(top of the hill)

### Action Space
{1,2}

### Sample Action
0->Moving down 1->Moving up

### Reward Function
Reward: +1 if the agent reaches goal state. 0 if the agent reaches the hole state.

### Graphical Representation
![exp-1](https://github.com/user-attachments/assets/3274cc22-eea7-4302-b6a8-d2a879abdd34)



## PYTHON REPRESENTATION:
```python
import gym
import gym_walk
P={0: {0: [(1.0, 0, 0.0, True)],
       1: [(1.0, 0, 0.0, True)]},
   1: {0: [(0.67, 0, 0.0, True),(0.33,2,1,True)],
       1: [(0.67, 2, 1.0, True),(0.33,0,0,True)]},
   2: {0: [(1.0, 2, 0.0, True)],
       1: [(1.0, 2, 0.0, True)]}
  }
```

## OUTPUT:

<img width="1834" height="543" alt="image" src="https://github.com/user-attachments/assets/dbb293e8-1c08-4e95-8861-69be118a68e1" />


## RESULT:
Thus the given real world problem is successfully represented in a MDP form .

