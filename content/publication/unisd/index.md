---
title: 'UniSD: Towards a Unified Self-Distillation Framework for Large Language Models'

authors:
  - Yiqiao Jin
  - admin
  - Lucheng Fu
  - Yijia Xiao
  - Yinyi Luo
  - Haoxin Liu
  - B. Aditya Prakash
  - Josiah Hester
  - Jindong Wang
  - Srijan Kumar

author_notes:
  - 'Equal contribution'
  - 'Equal contribution'

date: '2026-05-07T00:00:00Z'
doi: '10.48550/arXiv.2605.06597'
publishDate: '2026-05-07T00:00:00Z'

publication_types: ['article']
publication: 'arXiv preprint'
publication_short: 'arXiv'

abstract: 'Self-distillation (SD) offers a promising path for adapting large language models (LLMs) without relying on stronger external teachers. However, SD in autoregressive LLMs remains challenging because self-generated trajectories are free-form, correctness is task-dependent, and plausible rationales can still provide unstable or unreliable supervision. Existing methods mainly examine isolated design choices, leaving their effectiveness, roles, and interactions unclear. In this paper, we propose UniSD, a unified framework to systematically study self-distillation. UniSD integrates complementary mechanisms that address supervision reliability, representation alignment, and training stability, including multi-teacher agreement, EMA teacher stabilization, token-level contrastive learning, feature matching, and divergence clipping. Across six benchmarks and six models from three model families, UniSD reveals when self-distillation improves over static imitation, which components drive the gains, and how these components interact across tasks. Guided by these insights, we construct UniSD_full, an integrated pipeline that achieves the strongest overall performance, improving over the base model by +5.4 points and the strongest baseline by +2.8 points.'

summary: 'A unified framework that systematically studies self-distillation for large language models, integrating complementary mechanisms for supervision reliability, representation alignment, and training stability.'

tags:
  - Large Language Models
  - Self-Distillation
  - Model Adaptation

featured: true

url_pdf: 'https://arxiv.org/abs/2605.06597'
url_code: 'https://github.com/Ahren09/UniSD'
url_project: 'https://unifiedsd.github.io/'

image:
  caption: 'Overview of the UniSD framework (adapted from Figure 1 of the paper).'
  focal_point: 'Smart'
  preview_only: false
  alt_text: 'Diagram of the unified UniSD self-distillation framework and its component mechanisms.'

projects: []
slides: ""
---

## Abstract

Self-distillation offers a promising path for adapting large language models without stronger external teachers, but it remains hard to apply reliably in autoregressive LLMs. We propose **UniSD**, a unified framework that systematically studies self-distillation by integrating complementary mechanisms — multi-teacher agreement, EMA teacher stabilization, token-level contrastive learning, feature matching, and divergence clipping. Across six benchmarks and six models from three families, UniSD clarifies when and why self-distillation helps, and its integrated pipeline improves over the base model by +5.4 points and the strongest baseline by +2.8 points.
