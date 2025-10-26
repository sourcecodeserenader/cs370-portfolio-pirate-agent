# CS-370 Project Two - Pirate Intelligent Agent (Deep Q-Learning)
Student: Brianna Reed  
Course: CS-370 Current/Emerging Trends in CS  
Project: Treasure Hunt Game - Intelligent Agent (Pirate) using Deep Q-Learning

## Repo Contents
- `TreasureHuntGame.ipynb` - Jupyter Notebook source
- `Brianna_Reed_ProjectTwo.ipynb` - Exported HTML of the notebook (submission copy)
- `Brianna_Reed_ProjectTwo_DesignDefense.docx` - 2–3 page design defense

## How to Run (Instructor Notes)
1. Open `TreasureHuntGame.ipynb` in Jupyter.
2. Run Kernel → Restart & Run All.
3. Training will run; final cells should print:  
   - `Passes completion_check from all free starts? -> True`  
   - `Greedy play from (0,0) wins? -> True`

## Technical Summary
- Algorithm: Deep Q-Learning (experience replay, ε-greedy, MLP with PReLU)
- Goal: Learn a policy for the pirate to reach treasure from any free start cell
- Early stop: win_rate > 0.90 + `completion_check()` passes
- Files: only the notebook was modified; project .py helpers left unchanged

---

## Journal Reflection (Module Eight)
Briefly explain what you did on this project. What code were you given? What code did you create yourself?  
I completed the deep Q-learning training block in the provided notebook, implemented the neural network with Keras, added ε-decay and replay, and created helper functions (`train`, `dtrain`, `completion_check`, `play_game`). Starter files (`TreasureMaze.py`, `GameExperience.py`) were not modified.

Connect your learning to the larger field of computer science.
- What do computer scientists do and why does it matter?  
  We design systems that turn ambiguous real-world problems into computable tasks. Here, a maze becomes states, actions, and rewards letting an agent learn to act optimally.
- How do I approach a problem as a computer scientist?  
  By modeling, iterating, measuring, and improving: specify state/action spaces, choose an algorithm, run experiments, evaluate metrics, and refine.
- What are my ethical responsibilities to end users and the organization?  
  Ensure transparency, data minimization, accessibility, and fairness; document limitations; avoid overclaiming; and keep humans in the loop for critical decisions.

