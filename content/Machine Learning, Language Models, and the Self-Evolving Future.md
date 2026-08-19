---
date: 2026-08-20
tags:
  - ML
---
# About Machine Learning

The model arch determines the model's capability (limit, upper-bound).

Training data determines what capability the model may learn.

Training recipe (training settings, procedure, etc.) determines the efficiency of learning process.

# About Language Models

LLMs are just *Transformers trained with text data to maximize next-token probability*.

The process is just regular machine learning, with a self-supervised objective.

What makes it vital is the *emergence of capabilities* during scaling.

# About Self-Evolving

We can count on scaling with supervised learning and keep producing data.

However, self-evolving methods will *accelerate* intelligence process.

Reinforcement learning tried, but still
- requires a reward, which needs to be provided by human; and is often task-specific, limiting the scope of general learning
- pure exploration on high-dimentional decision space, with insufficient semantical exploration structure (also refered to as *common sense*).

Self-supervised learning leverages an objective for capturing the capabilities within data. Together with scaling, it provides a probability towards self-evolving.

We've found the next-token probability objective for LLMs. Now we only need to find another for the temporal, multi-modal data of the physical world.