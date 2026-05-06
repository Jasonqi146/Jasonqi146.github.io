---
layout: page
title: Agentic RL Infrastructure
description: Distributed post-training systems for terminal and coding agents at Snorkel AI.
importance: 1
eyebrow: Snorkel AI
accent: ink
stack:
  - Ray
  - Kubernetes
  - verl
  - GRPO
  - Containerized rollouts
highlight: Built multi-node RL infrastructure spanning 64 H200 GPUs and 6,000+ rollout environments for long-horizon agent training.
---

At Snorkel AI, I have been building the machinery that makes agentic RL experiments possible at useful scale: distributed training, asynchronous rollouts, terminal environments, container lifecycle management, registry and filesystem caching, and failure-mode observability.

The research point is not only throughput. Long-horizon agent training creates a measurement problem: failures can come from the environment, tool execution, reward signal, policy behavior, orchestration, or tail latency. A useful system has to make those failures visible enough that model improvement is not confused with infrastructure luck.

This work connects my systems taste with my evaluation taste: the better the rollout and logging infrastructure, the more precisely we can ask which feedback signals actually improve agent behavior.
