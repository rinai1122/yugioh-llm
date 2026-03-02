# Agent Types and Comparisons

This document outlines the different types of players and agents we are evaluating in this research project.

## 1. LLM-Based Agents (Our Focus)
Our primary objective is to develop and evaluate Large Language Model (LLM) based agents for playing Yu-Gi-Oh!. 
**Advantages:**
- Can interpret complex, unstructured card texts naturally.
- Can leverage broad reasoning capabilities for deck building and novel strategies.
- Easily adaptable without extensive retraining for new card releases or custom formats.

**Challenges:**
- Context window limits when tracking game state, graveyard, and large card pools.
- Hallucination of game rules or card effects.
- Reasoning speed and inference cost compared to traditional RL models.

## 2. Reinforcement Learning (RL) Based Agents (Baselines)
Currently existing AI for Yu-Gi-Oh! heavily relies on RL and search algorithms (like MCTS).
**Role in Research:**
- Serve as the primary automated baseline to measure LLM performance.
**Characteristics:**
- Excellent at specific mathematical optimizations and known combinatorial setups.
- Often rigid; adapting to new cards or massive rule changes requires significant engine modification or retraining.
- Lacks semantic understanding of the cards, relying solely on game engine simulations.

## 3. Human Players
The ultimate benchmark for generalizability and strategic depth.
**Role in Research:**
- To determine if the LLM can achieve superhuman performance or at least competitive expert-level play.
**Characteristics:**
- Strong intuition for meta-game and opponent psychology (bluffing, reading delays).
- Capable of long-term strategic planning and highly creative deck building.
