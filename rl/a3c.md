# Asynchronous Methods for Deep Reinforcement Learning

## Abstract
We propose a conceptually simple and lightweight framework for deep reinforcement learning 
that uses asynchronous gradient descent for optimization of deep neural network controllers. 
We present asynchronous variants of four standard reinforcement learning algorithms and 
show that parallel actor-learners have a stabilizing effect on training allowing all four methods 
to successfully train neural network controllers. 
The best performing method, an asynchronous variant of actor-critic, surpasses the current state-of-the-art 
on the Atari domain while training for half the time on a single multi-core CPU instead of a GPU. 
Furthermore, we show that asynchronous actor-critic succeeds on a wide variety of continuous motor control problems 
as well as on a new task of navigating random 3D mazes using a visual input.

## Introduction
* Online RL algorithms with deep neural networks is unstable.
* A variety of solutions have been proposed by aggregating over memory for reducing non-stationarity of the RL agent and decorrelating updates.
* This "limits the methods to off-policy reinforcement learning algorithms."
* Experience replay has drawbacks: more memory, computation and off-policy learning algorithms.
* We ***asynchronously execute multiple agents in parallel, on multiple instances of the environment.***
* It also alleviates the problem of online RL algorithms with much less sophisticated hardware.

## Related Work
* Gorila (General Reinforcement Learning Architecture) performs asynchronous training
  * Gradients are asynchronously sent to a central parameter server
  * Outperformed DQN over 49 Atari games.
* Parallelizing approaches: Map Reduces framework, or peer-to-peer communicating multiple actor-learners
* Convergence property of distributed Q-learning was investigated.
* Evolutionary methods also have been applied to RL tasks.

## Reinforcement Learning Background

## Asynchronous RL Framework

## Experiments

## Conclusion and Discussion
