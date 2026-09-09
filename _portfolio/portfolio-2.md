---
title: "Traffic Sign Recognition & Computer Vision CNN Benchmark"
excerpt: "Custom annotated dataset curation and benchmark comparing Classical Machine Learning (SVM/Random Forest) with Deep Convolutional Neural Networks, reaching 97.35% accuracy.<br/><img src='/images/traffic_signs_detection.jpg' width='100%'>"
collection: portfolio
category: "projects"
order: 5
---

{% include base_path %}

<div class="project-media-container" style="max-width: 680px; margin: 20px 0;">
  <img src="{{ base_path }}/images/traffic_signs_detection.jpg" alt="Traffic Signs Detection Benchmark" style="width: 100%; border-radius: 12px;">
</div>

### Executive Summary
Engineered an end-to-end computer vision recognition pipeline to detect and classify multi-class traffic signs under severe environmental noise (motion blur, lighting variations, partial occlusions).

---

### Methodology & Technical Innovations

1. **Dataset Curation & Data Augmentation:**
   - Curated a tailored dataset of road sign classes.
   - Built a robust data augmentation pipeline applying affine transformations, synthetic Gaussian blur, chromatic aberration, and perspective warping to prevent overfitting.

2. **Benchmarking Classical ML vs Deep CNNs:**
   - **Classical ML Baseline:** Feature extraction via Histogram of Oriented Gradients (HOG) and color histograms fed into tuned Support Vector Machines (SVMs) and Random Forests.
   - **Deep CNN Architecture:** Multi-layer convolutional feature extractor with batch normalization, dropout regularization, and adaptive average pooling.

---

### Empirical Results & Takeaways
- Achieved **97.35% test classification accuracy** with the CNN architecture.
- Demonstrated significantly higher prediction confidence and calibration stability across low-contrast test samples compared to classical ML approaches.
- **Tech Stack:** `OpenCV`, `PyTorch`, `Scikit-learn`, `Matplotlib`, `NumPy`.
