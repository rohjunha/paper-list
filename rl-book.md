# Reinforcement Learning: An Introduction
## Table of contents
  1. [The Reinforcement Learning Problem](#the-reinforcement-learning-problem)
    1. [Reinforcement Learning](#reinforcement-learning)
    1. [Elements of Reinforcement Learning](#elements-of-reinforcement-learning)
    1. [Limitations and Scope](#limitations-and-scope)
    1. [An Extended Example: Tic-Tac-Toe](#an-extended-example-tic-tac-toe)

## The Reinforcement Learning Problem
### Reinforcement Learning
These three characteristics— being closed-loop in an essential way, not having direct instructions as to what actions to take, and where the consequences of actions, including reward signals, play out over extended time periods—are the three most important distinguishing features of the reinforcement learning problem.

Another key feature of reinforcement learning is that it explicitly considers the whole problem of a goal-directed agent interacting with an uncertain environment.

### Elements of Reinforcement Learning
Beyond the agent and the environment, one can identify four main subelements of a reinforcement learning system:
* a policy
* a reward signal
* a value function

and, optionally
* a model of the environment.

A ***policy*** defines the learning agent’s way of behaving at a given time. Roughly speaking, a policy is a mapping from perceived states of the environment to actions to be taken when in those states.

A ***reward signal*** defines the goal in a reinforcement learning problem. On each time step, the environment sends to the reinforcement learning agent a single number, a reward. The agent’s sole objective is to maximize the total reward it receives over the long run. The reward signal thus defines what are the good and bad events for the agent.

Whereas the reward signal indicates what is good in an immediate sense, a ***value function*** specifies what is good in the long run. Roughly speaking, the value of a state is the total amount of reward an agent can expect to accumulate over the future, starting from that state.

### Limitations and Scope
### An Extended Example: Tic-Tac-Toe
