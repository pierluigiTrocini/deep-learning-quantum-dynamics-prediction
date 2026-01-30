# Deep Learning for Forecasting Quantum Dynamics
---
### Try the Code
You can view, build, and test the model on a sample dataset via the following Google Colab notebook:

[**Link to Colab Notebook**](https://colab.research.google.com/drive/1hPapB9t0jAlh8-TPx8QdAbKggoulihlh?usp=sharing)
---
This project presents a **Deep Learning** framework designed to model and forecast the temporal evolution of multi-qubit quantum systems. The primary goal is to bypass the computational bottlenecks of classical simulations, which face exponential complexity due to quantum entanglement.

## Context and Motivation
With the rise of advanced quantum processors, such as Google's Willow, the ability to accurately track quantum state dynamics has become essential. Since classical simulations struggle with chips exceeding 100 qubits, this study leverages neural architectures to bypass traditional simulation limits and facilitate the design of next-generation quantum hardware.

## Features and Implementation
The framework integrates several advanced AI techniques applied to quantum physics:

* **Predictive Models**: Implementation and comparison of **LSTM** (Long Short-Term Memory) and **Transformer** architectures to capture recurrent and non-local temporal dependencies in quantum trajectories.
* **Time Window Optimization**: Analysis to identify optimal input windows (20 and 50 timesteps), balancing short-term dynamic agility with the context needed to mitigate long-term divergence.
* **Curriculum Learning Strategy**: The training follows a three-phase strategy: one-step prediction, handling corrupted inputs (20% random masking), and autoregressive rollout over a 10-step horizon to ensure physical stability.
* **Super-Resolution (SR) Module**: A hybrid architecture using **Conv1DTranspose** and residual connections to reconstruct high-resolution sequences (100 steps) from low-resolution inputs (50 steps), preserving vital high-frequency oscillations.
* **Explainability**: Analysis of **Attention Maps** to verify that the model correctly learns physical principles such as temporal locality and causality.

## Key Results
* **Transformers** demonstrated superior scalability and interpretability through self-attention mechanisms compared to LSTMs.
* The **Super-Resolution** module achieved high fidelity in reconstructing micro-temporal details, maintaining physical consistency across various signal morphologies.

---

### Authors
* **Emanuele Colecchia** (ID: 276527)
* **Pierluigi Trocini** (ID: 280977)
* **Date**: January 30, 2026
