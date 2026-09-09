---
title: "Specialized QA System with Llama-3.2-3B (Top 3 Kaggle Finish)"
excerpt: "Hybrid RAG + Q-LoRA alignment on temporal question answering datasets, achieving a 450x relative F1-score leap from 0.001 to 0.456 and securing a Top 3 finish in a Kaggle AI competition."
collection: portfolio
category: "projects"
order: 2
---

{% include base_path %}

### 🏆 Executive Summary & Impact
In this competitive AI challenge, the objective was to construct a highly accurate Question-Answering system capable of reasoning over nuanced, temporal knowledge bases. Out-of-the-box pretrained LLMs suffer from severe hallucinations and lack of temporal grounding (baseline F1 ~ 0.001). 

By architecting a hybrid **Retrieval-Augmented Generation (RAG)** pipeline combined with **Parameter-Efficient Fine-Tuning (Q-LoRA)**, this solution achieved an **F1-score of 0.456**, securing a **Top 3 finish on the global Kaggle leaderboard**.

---

### Technical Architecture

1. **Vector Retrieval & Contextual Reranking:**
   - Chunked and embedded temporal knowledge documents into high-dimensional dense vector embeddings.
   - Built an automated retrieval mechanism to supply the LLM with time-anchored evidence passages.

2. **Parameter-Efficient Fine-Tuning (Q-LoRA):**
   - Quantized the base **Llama-3.2-3B-Instruct** backbone to 4-bit precision via NormalFloat4 (NF4) with double quantization.
   - Attached low-rank adapter matrices (LoRA rank r = 16, &alpha; = 32) to query/key/value attention projections.
   - Supervised fine-tuning using Hugging Face `peft` and `trl` frameworks.

---

### Key Takeaways
- Proven ability to drastically enhance LLM domain-specific accuracy under compute constraints.
- Demonstrates mastery of modern generative AI workflows: PyTorch, Hugging Face, Transformers, Q-LoRA, bitsandbytes, and RAG.
