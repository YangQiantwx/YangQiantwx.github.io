---
layout: essay
type: essay
title: "Hashtag2Action: Data Engineering and Self-Supervised Pre-Training for Action Recognition in Short-Form Videos"
date: 2025-10-19
published: true
labels:
  - Foundation Models
  - Action Recognition
  - VideoMAE
  - Self-Supervised Learning
  - ICCV 2025
---

<img src="/img/foundation-models/clipsamples.jpeg" alt="Example TikTok video clips used for pretraining" class="img-fluid rounded shadow my-3" style="max-width: 700px;">

### Abstract

Developing video action recognition models that capture real-world human behavior while addressing social and ethical considerations is crucial for advancing AI. We present a comprehensive data-engineering pipeline that leverages weakly labeled, culturally diverse short videos from social media (e.g., TikTok) to curate a dataset of 283,582 clips spanning 386 action groups with minimal human intervention. Our pipeline employs adaptive hashtag selection, metadata filtering, and vision-based frame selection to ensure high-quality data. Building on this curated dataset, we introduce a self-supervised pre-training framework using the VideoMAE V2 [Wang et al., 2023] backbone. Fine-tuning on UCF101 [Soomro et al., 2012], HMDB51 [Kuehne et al., 2011], Kinetics-400 [Kay et al., 2017], and Something-Something V2 [Goyal et al., 2017] yields competitive results—99.05%, 86.08%, 85.51%, and 74.27% accuracy, respectively—using only 20% of the original pre-training data. Our findings illustrate that self-supervised learning on carefully curated weakly labeled data can achieve robust downstream performance without human annotation, enabling the use of rich social media data in a privacy-conscious manner. We open-source our data engine and fine-tuning framework to streamline data curation on short-video platforms and accelerate future research in human-centric video recognition.

### Publication

**Accepted at**: *Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV) Workshops — The First Workshop on Short-Form Video Understanding (SVU 2025), Honolulu, Hawai‘i, USA.*  
**PDF (Open Access)**: [View on CVF](https://openaccess.thecvf.com/content/ICCV2025W/SVU/papers/Qian_Hashtag2Action_Data_Engineering_and_Self-Supervised_Pre-Training_for_Action_Recognition_in_ICCVW_2025_paper.pdf){:target="_blank"}

### Comments

- **Data pipeline innovation**: Adaptive hashtag selection and vision-based frame filtering ensure both cultural diversity and data quality.  
- **Ethical sourcing**: Weak labels and minimal manual curation support privacy-conscious large-scale pretraining.  
- **SSL impact**: Demonstrates that modern self-supervised objectives can match or exceed supervised baselines with far less annotated data.  
- **Open science**: Engine and framework released open-source to lower barriers for future video-based foundation model research.  
