---
title: UniSD
summary: A unified framework for studying self-distillation in large language models.
tags:
  - Large Language Models
date: 2026-05-07
featured: false

image:
  caption: 'Overview of the UniSD framework (adapted from the paper).'
  focal_point: Smart
  preview_only: false
  alt_text: 'UniSD unified self-distillation framework diagram.'

links:
  - name: Paper
    url: https://arxiv.org/abs/2605.06597
  - name: Code
    url: https://github.com/Ahren09/UniSD
  - name: Project
    url: https://unifiedsd.github.io/
url_pdf: 'https://arxiv.org/abs/2605.06597'
url_code: 'https://github.com/Ahren09/UniSD'
url_project: 'https://unifiedsd.github.io/'
---

Self-distillation lets large language models improve without a stronger external teacher, but it is hard to apply reliably: self-generated trajectories are free-form, correctness is task-dependent, and prior work studies design choices in isolation. **UniSD** is a unified framework that brings these choices together — multi-teacher agreement, EMA teacher stabilization, token-level contrastive learning, feature matching, and divergence clipping — to study when and why self-distillation helps.

**My role.** I am a co-author on this collaboration. Across six benchmarks and six models from three families, UniSD clarifies which components drive gains and how they interact, and its integrated pipeline improves over the base model by +5.4 points and over the strongest baseline by +2.8 points.
