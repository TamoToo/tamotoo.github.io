---
title: "From-Scratch Deep Learning & RL Implementations (Transformers, DQN, DDPG)"
excerpt: "From-scratch PyTorch implementations of Transformer foundations (BERT, GPT-2) and continuous/discrete RL control agents (DQN, DDPG) with live W&B telemetry.<br/><video width='100%' autoplay muted loop playsinline><source src='/images/CarRacing-v3.mp4' type='video/mp4'></video>"
collection: portfolio
category: "projects"
order: 4
---

{% include base_path %}

<div class="project-media-container" style="max-width: 680px; margin: 20px 0;">
  <video autoplay muted loop playsinline style="width: 100%; border-radius: 12px;">
    <source src="{{ base_path }}/images/CarRacing-v3.mp4" type="video/mp4">
  </video>
</div>

### Executive Summary
A comprehensive deep-dive into fundamental algorithmic implementations in **PyTorch**, written from mathematical first principles rather than off-the-shelf high-level libraries. This project covers both foundational **Generative Language Models / Transformers** and state-of-the-art **Reinforcement Learning** agents.

---

### Key Implementations

#### 1. Reinforcement Learning Foundations
- **DQN (Deep Q-Network):** Implemented experience replay memory, target network stabilization, &epsilon;-greedy exploration decay, and Bellman error backpropagation. Evaluated on discrete environments (CartPole, LunarLander).
- **DDPG (Deep Deterministic Policy Gradient):** Actor-Critic architecture for continuous action spaces featuring Ornstein-Uhlenbeck exploration noise and soft target updates (&tau; ≪ 1). Mastered the **OpenAI Gymnasium CarRacing-v3** continuous driving environment.

#### 2. Transformer Architectures (From Scratch)
- **BERT (Bidirectional Encoder Representations from Transformers):** Multi-head self-attention mechanisms, learned positional embeddings, layer normalization, and Masked Language Modeling (MLM) pre-training pipelines.
- **GPT-2 (Causal Generative Pre-training):** Autoregressive masked self-attention blocks, residual projections, and top-k / top-p nucleus sampling decoders.

---

### Telemetry & MLOps
- Full hyperparameter tracking, loss curve monitoring, gradient norm analysis, and reward convergence visualization via **Weights & Biases (W&B)**.
