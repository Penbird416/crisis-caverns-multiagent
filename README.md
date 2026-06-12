# Crisis Caverns — Multi-Agent Reinforcement Learning

A multi-objective, multi-agent reinforcement learning system built inside a cave-collapse environment. Three specialized agents with competing objectives must be coordinated in real time under uncertainty.

## What it does

After a cave collapse, an agentic AI explorer must navigate competing survival objectives simultaneously:

| Agent | Objective |
|---|---|
| Goal-Seeking Agent | Reach the exit |
| Reward-Seeking Agent | Collect energy crystals |
| Damage-Avoidance Agent | Avoid hostile cave creatures |
| Coordinator | Combine all three into a single action per step |

The system explores how **multi-objective RL** handles value trade-offs — the weights assigned to each objective encode real-world priorities about what an autonomous agent should optimize for.

## Key concepts

- Multi-objective reward vectors (vs scalar reward)
- Coordinator pattern for multi-agent action aggregation
- Escape success / coins collected / monster hits / steps as evaluation dimensions
- Checkpoint-based evaluation of reward design decisions

## Stack

- Python 3.10+
- NumPy
- Custom game environment (no external RL library required)

## Setup

```bash
pip install -r requirements.txt
jupyter notebook crisis_caverns_multiagent.ipynb
```

No API keys required.
