# Research Plans

This outline details the roadmap for developing and evaluating LLM-based agents in the Yu-Gi-Oh! environment.

## Phase 1: Environment and Baseline Setup
- Integrate with the [ygo-agent](https://github.com/sbl1996/ygo-agent) core engine.
- Establish standard RL baselines for performance comparison.
- Define evaluation metrics (win rate, action validity, turn execution time).

## Phase 2: LLM Gameplay Integration
- **State Translator:** Convert the YGOPro/ygo-agent engine state into structured text prompts for the LLM.
- **Action Parser:** Map LLM text outputs to valid game engine actions (summons, activations, phases).
- **Context Management:** Implement memory architecture for the LLM to track board state across turns.
- Conduct initial tests against random agents and weak RL agents.

## Phase 3: Deck Building Module
- **Objective:** The LLM must not only play but also intelligently construct viable decks.
- Provide the LLM with accessible card database embeddings.
- Prompt engineering for synergy identification, level/scale curves, and archetype matching.
- Create automated tournaments where the LLM builds a deck from scratch and plays it against known meta decks.

## Phase 4: Comparative Evaluation
- **LLM vs RL:** Run thousands of simulated matches to achieve statistical significance. Compare different LLM sizes/families.
- **LLM vs Human:** Organize exhibition matches against proficient human players.
- Evaluate adaptability: Test how quickly the LLM can adapt to newly introduced custom cards compared to an RL agent.

## Phase 5: Advanced Tactics & Continuous Improvement
- Refine reasoning through Chain-of-Thought (CoT) and ReAct prompting.
- Implement post-match self-reflection steps to adjust strategies and refine deck compositions over time.
