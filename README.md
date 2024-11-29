# Nim - An AI Project

This project is a part of the CS50 AI course, where I developed an AI that learns to play the game of Nim using reinforcement learning. The AI improves its strategy by playing against itself multiple times and eventually plays very well against a human opponent.

## Table of Contents
- [Introduction](#introduction)
- [How it Works](#how-it-works)
  - [Game of Nim](#game-of-nim)
  - [Reinforcement Learning](#reinforcement-learning)
- [Training the AI](#training-the-ai)
- [Playing Against the AI](#playing-against-the-ai)

## Introduction
The game of Nim is a mathematical strategy game where players take turns removing objects from heaps or piles. On each turn, a player must remove at least one object from a single pile, and they may remove any number of objects provided they all come from the same pile. The player forced to take the last object loses.

In this project, I implemented a reinforcement learning agent that learns to play Nim by improving its strategy through self-play.

## How it Works
### Game of Nim
The game is initialized with a set of piles, each containing a certain number of objects. Players take turns removing any number of objects from any of the piles. The player forced to remove the last object loses the game.

### Reinforcement Learning
The AI uses Q-learning, a type of reinforcement learning, to learn the best moves in different states of the game. The AI updates its knowledge base (The Q-Values) based on the rewards it receives. I have also implemented _epsilon-greedy-approach_ to balance between exploration and exploitation, letting the AI to explore new states and actions randomly with some probability.

The Q-values (rewards) are represented as a dictionary with keys represented _(state, action)_ pairs

## Training the AI
the _train()_ function simulates a number of games where the AI plays against itself. During each game, the AI updates its Q-values based on the rewards it receives. The more games it plays, the better it gets at making optimal moves

## Playing Against the AI
the _play()_ functions allows a human player to compete against the trianed AI



