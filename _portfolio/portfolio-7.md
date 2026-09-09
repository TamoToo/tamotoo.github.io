---
title: "ClimbVision AI: Computer Vision & Multi-Agent Climbing Analysis"
excerpt: "YOLO hold segmentation and spatial route modeling with NetworkX, paired with a stateful LangGraph agent (GPT-4o) and high-performance FastAPI backend."
collection: portfolio
category: "projects"
order: 1
---

{% include base_path %}

### Overview
ClimbVision AI is an intelligent climbing route analysis system designed to understand climbing problems through multi-modal perception and graph reasoning.

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
