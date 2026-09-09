---
title: "24h Spatio-Temporal Wind Power Forecasting (NVIDIA H100 HPC Clusters)"
excerpt: "Hybrid CNN-LSTM Seq2Seq architecture integrating high-resolution Numerical Weather Prediction grids to achieve a 60% reduction in MAE over baseline LSTM models."
collection: portfolio
category: "internships"
order: 1
---

{% include base_path %}

### ⚡ Research Internship — Polytechnique Montréal
*Jan 2026 – May 2026* | **Role:** AI Research Engineer

---

### Challenge & Motivation
Accurately predicting 24-hour wind power generation is critical for modern green energy grid balancing. Standard univariate or naive recurrent models fail to capture the complex multi-scale spatio-temporal dynamics of localized wind shear and high-dimensional atmospheric weather grids.

---

### Architectural Innovation: Hybrid CNN-LSTM Seq2Seq
1. **Spatial Feature Extraction (CNN Front-End):**
   - Ingested multi-channel 2D spatial meteorological grids (Numerical Weather Prediction - NWP).
   - Utilized convolutional filters to extract high-level atmospheric pressure gradients and localized wind vectors.

2. **Temporal Modeling (LSTM Seq2Seq):**
   - Fed the spatial representations into an Encoder-Decoder recurrent network equipped with temporal attention to model the 24-hour autoregressive sequence.

3. **High-Performance Distributed Training (NVIDIA H100):**
   - Scaled data-parallel training across **NVIDIA H100 GPU clusters**.
   - Executed automated Bayesian hyperparameter sweeps to maximize generalization across changing seasonal weather patterns.

---

### Empirical Impact
- **60% reduction in Mean Absolute Error (MAE)** compared to standard LSTM baselines.
- Scalable pipeline capable of real-time multi-turbine distributed inference.
