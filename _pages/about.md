---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

I am an **AI Engineer and Machine Learning Researcher** graduated from a Master's Double Degree in Computer Engineering at **[Polytechnique Montréal](https://www.polymtl.ca/)** (specializing in Artificial Intelligence and Deep Learning) and **[Université de Technologie de Compiègne (UTC)](https://www.utc.fr/)** (specializing in Data Science & AI).

My work centers on **Reinforcement Learning**, **Fine-Tuned LLMs & Multi-Agent Systems**, and **Spatio-Temporal Deep Learning on HPC infrastructure**. I enjoy building systems from foundational algorithms up to scalable production pipelines. I am deeply passionate about **AI research for real-world applications**, particularly in **energy, climate, and environmental sustainability**.

<div style="margin: 16px 0 24px;">
  <a href="{{ site.baseurl }}{% link files/CV_English_Forest_Thomas.pdf %}" target="_blank" class="btn-cv-download">
    <i class="fa fa-file-pdf"></i> Download Resume (EN)
  </a>
  <a href="{{ site.baseurl }}{% link files/CV_Francais_Forest_Thomas.pdf %}" target="_blank" class="btn-cv-download">
    <i class="fa fa-file-pdf"></i> Télécharger CV (FR)
  </a>
</div>

---

### Highlights & Key Results

* <span class="highlight-badge">🏆 Top 3 Kaggle</span> **Specialized QA System with Llama-3.2-3B:** Aligned Llama-3.2 using hybrid Retrieval-Augmented Generation (RAG) and parameter-efficient fine-tuning (Q-LoRA) on temporal question-answering benchmarks, securing a Top 3 rank in a competitive Kaggle tournament.
* <span class="highlight-badge">⚡ -60% MAE</span> **24h Spatio-Temporal Wind Power Forecasting:** Architected and optimized a hybrid CNN-LSTM Seq2Seq framework in PyTorch integrating high-resolution NWP weather grids on **NVIDIA H100 GPU clusters** at Polytechnique Montréal, reducing MAE by 60% vs. baseline LSTM models.
* <span class="highlight-badge">🧗 Vision &amp; Agents</span> **[ClimbVision AI](https://climbvision-ai-beta.vercel.app):** Developed a computer vision YOLO pipeline to segment climbing holds, modeled routes as directed spatial graphs with NetworkX, and engineered a stateful multi-agent system with LangGraph (GPT-4o) and FastAPI — **[Live Web App ↗](https://climbvision-ai-beta.vercel.app)**.
* <span class="highlight-badge">🤖 Embedded C++</span> **PocketCompanion:** Built a portable, touch- and motion-reactive digital companion on an ESP32-S3 circular touch display with a 60 FPS LVGL avatar engine, 6-axis IMU physics, and a Python JSON-to-C++ code generator.
* <span class="highlight-badge">🧠 Cognitive AI</span> **Human Behavior Simulation &amp; Custom Gymnasium (CEA-List):** Developed numerical simulations of human decision-making using the SOAR cognitive architecture and engineered a custom OpenAI Gymnasium simulation pipeline from scratch in Python to benchmark RL agents.
* <span class="highlight-badge">📊 Deep RL</span> **From-Scratch Deep Learning &amp; RL:** Implemented Transformer architectures (BERT, GPT-2) and continuous/discrete RL agents (DQN, DDPG) in PyTorch with telemetry tracked on Weights &amp; Biases.
* <span class="highlight-badge">🎖️ Top 5 Finish</span> **AI Agent for Board Game (Divercité):** Developed a competitive game-playing agent using Min-Max search with Alpha-Beta pruning and policy-guided reinforcement learning heuristics.
* <span class="highlight-badge">🎯 97.35% Acc</span> **Traffic Sign Perception System:** Trained CNN models on a curated annotated dataset with geometric and lighting distortions, benchmarking Classical ML against Deep CNNs.

---

### Selected Projects

Detailed writeups and media demonstrations are available in the [Portfolio]({{ site.baseurl }}/portfolio/):
- **[ClimbVision AI]({{ site.baseurl }}/portfolio/portfolio-7/):** YOLO hold segmentation + NetworkX spatial graphs + LangGraph multi-agent reasoning ([**Live Web App ↗**](https://climbvision-ai-beta.vercel.app)).
- **[PocketCompanion]({{ site.baseurl }}/portfolio/portfolio-8/):** Interactive ESP32-S3 embedded companion with 60 FPS LVGL procedural animation and IMU physics.
- **[From-Scratch Deep RL &amp; Transformers]({{ site.baseurl }}/portfolio/portfolio-1/):** PyTorch implementations of BERT, GPT-2, DQN, and DDPG on Gym CarRacing with live video.
- **[Traffic Sign Detection Benchmark]({{ site.baseurl }}/portfolio/portfolio-2/):** Multi-class CNN vs. Classical ML perceptual pipeline.

---

### Contact

- **Email:** [t.forest0573@gmail.com](mailto:t.forest0573@gmail.com)
- **GitHub:** [@TamoToo](https://github.com/TamoToo)
- **Location:** France