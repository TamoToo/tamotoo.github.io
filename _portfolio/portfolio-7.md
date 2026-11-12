---
title: "ClimbVision AI: Computer Vision & Multi-Agent Climbing Analysis"
excerpt: "YOLO hold segmentation and spatial route modeling with NetworkX, paired with a stateful LangGraph agent (GPT-4o) and high-performance FastAPI backend.<br/><a href='https://climbvision-ai-beta.vercel.app' target='_blank' rel='noopener noreferrer' class='btn-cv-download' style='margin-top: 10px;'><i class='fas fa-external-link-alt'></i> Launch Live Web App (climbvision-ai-beta.vercel.app)</a>"
collection: portfolio
category: "projects"
order: 1
---

{% include base_path %}

<div style="margin: 12px 0 20px;">
  <a href="https://climbvision-ai-beta.vercel.app" target="_blank" rel="noopener noreferrer" class="btn-cv-download">
    <i class="fas fa-external-link-alt"></i> Launch Live Application (climbvision-ai-beta.vercel.app)
  </a>
</div>

### Overview
ClimbVision AI is an intelligent climbing route analysis system designed to understand climbing problems through multi-modal perception and graph reasoning.

- **Live Web Application:** [climbvision-ai-beta.vercel.app](https://climbvision-ai-beta.vercel.app)

---

### Technical Architecture

1. **Perception & Spatial Graph Modeling:**
   - Trained and fine-tuned a **YOLO** computer vision pipeline to detect and segment climbing holds with high geometric precision.
   - Modeled route topologies as directed spatial graphs with **NetworkX**, quantifying reachability, body positioning transitions, and move difficulty.

2. **Stateful Multi-Agent Reasoning (LangGraph & GPT-4o):**
   - Engineered an agentic reasoning workflow utilizing **LangGraph** to recommend move sequences and alternative beta solutions.
   - Deployed through an asynchronous, high-throughput **FastAPI** backend coupled with a responsive **Next.js** interface.

---

### Tech Stack
`YOLO`, `NetworkX`, `LangGraph`, `FastAPI`, `Next.js`, `Python`, `PyTorch`
