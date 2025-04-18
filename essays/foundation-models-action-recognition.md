---
layout: essay
type: essay
title: "Advancing Human Action Recognition with Foundation Models Trained on Unlabeled Public Videos"
date: 2024-02-19
published: true
labels:
  - Foundation Models
  - Action Recognition
  - VideoMAE
  - Self-Supervised Learning
---

<img src="/img/foundation-models/clipsamples.jpeg" alt="Example TikTok video clips used for pretraining" class="img-fluid rounded shadow my-3" style="max-width: 700px;">

### Abstract

The increasing variety and quantity of tagged multimedia content on online platforms offers a unique opportunity to advance the field of human action recognition. In this study, we utilize **283,582 unique, unlabeled TikTok video clips**, categorized into **386 hashtags**, to train a domain-specific foundation model for action recognition.

We employ **VideoMAE V2**, an advanced model integrating Masked Autoencoders (MAE) with Vision Transformers (ViT), pre-trained on this diverse collection of unstructured videos. Our model, fine-tuned on established action recognition benchmarks such as **UCF101** and **HMDB51**, achieves state-of-the-art results:

- **UCF101**: 99.05%  
- **HMDB51**: 86.08%  
- **Kinetics-400**: 85.51%  
- **Something-Something V2**: 74.27%  
(using the ViT-giant backbone)

These results highlight the potential of using unstructured and unlabeled videos as a valuable source of diverse and dynamic content for training foundation models.

---

### Key Findings

- 📉 Performance gains from additional pre-training data diminish as dataset size scales
- 🎯 Data *quality* is more critical than sheer quantity in self-supervised learning
- 🧠 Domain-specific pretraining leads to highly effective transfer learning for video understanding

---

### Relevance to PhD Research

This work contributes directly to my PhD focus on:
- Foundation models for healthcare and behavioral diagnostics
- Self-supervised video representation learning
- Scalability and efficiency of domain-specific pretraining

---

### Contribution

- Led the design, pretraining, and fine-tuning of foundation models
- Conducted benchmark evaluations across four major datasets
- Analyzed learning dynamics across dataset sizes
- Sole author of all written content and figures

---

### Preprint Access

📄 [arXiv:2402.08875](https://arxiv.org/abs/2402.08875){:target="_blank"}

This work is currently under review and available as a public technical report.
