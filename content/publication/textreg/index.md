---
title: 'TextReg: Mitigating Prompt Distributional Overfitting via Regularized Text-Space Optimization'

authors:
  - Lucheng Fu
  - Ye Yu
  - admin
  - Yiqiao Jin
  - Haibo Jin
  - B. Aditya Prakash
  - Haohan Wang

date: '2026-05-20T00:00:00Z'
doi: '10.48550/arXiv.2605.21318'
publishDate: '2026-05-20T00:00:00Z'

publication_types: ['article']
publication: 'arXiv preprint'
publication_short: 'arXiv'

abstract: 'Large language models (LLMs) are highly sensitive to the prompts used to specify task objectives and behavioral constraints. Many recent prompt optimization methods iteratively rewrite prompts using LLM-generated feedback, but the resulting prompts often become longer, accumulate narrow sample-specific rules, and generalize poorly beyond the training distribution. We study this failure mode as prompt distributional overfitting and argue that it reflects a lack of representation control in discrete text-space optimization. We formalize this view through representational inefficiency, a dual-factor measure that decomposes prompt inefficiency into capacity cost and scope narrowness. We propose TextReg, a regularization framework that realizes a soft-penalty objective through regularized textual gradients, combining Dual-Evidence Gradient Purification, Semantic Edit Regularization, and Regularization-Guided Prompt Update. Across multiple reasoning benchmarks, TextReg substantially improves out-of-distribution generalization, with accuracy gains of up to +11.8% over TextGrad and +16.5% over REVOLVE.'

summary: 'A regularization framework for text-space prompt optimization that mitigates distributional overfitting and improves out-of-distribution generalization.'

tags:
  - Large Language Models
  - Prompt Optimization

featured: false

url_pdf: 'https://arxiv.org/abs/2605.21318'
url_code: 'https://github.com/luchengfu6/TextReg'

image:
  caption: 'TextReg method overview (adapted from Figure 2 of the paper).'
  focal_point: 'Smart'
  preview_only: false
  alt_text: 'Diagram of the TextReg regularized prompt-optimization pipeline.'

projects: []
slides: ""
---

## Abstract

LLMs are highly sensitive to their prompts, and iterative prompt-optimization methods often overfit: prompts grow longer, accumulate sample-specific rules, and generalize poorly. We study this as **prompt distributional overfitting** and introduce **TextReg**, a regularization framework that realizes a soft-penalty objective through regularized textual gradients — combining Dual-Evidence Gradient Purification, Semantic Edit Regularization, and Regularization-Guided Prompt Update. Across reasoning benchmarks, TextReg improves out-of-distribution generalization by up to +11.8% over TextGrad and +16.5% over REVOLVE.
