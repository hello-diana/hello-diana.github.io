---
title: TextReg
summary: Regularized text-space prompt optimization that resists distributional overfitting.
tags:
  - Large Language Models
  - Prompt Optimization
date: 2026-05-20
featured: true

image:
  caption: 'Overfitted vs. generalizable prompts on an out-of-domain question (adapted from the paper).'
  focal_point: Smart
  preview_only: false
  alt_text: 'An out-of-domain question where an overfitted prompt fails and a generalizable prompt succeeds.'

links:
  - name: Paper
    url: https://arxiv.org/abs/2605.21318
  - name: Code
    url: https://github.com/luchengfu6/TextReg
url_pdf: 'https://arxiv.org/abs/2605.21318'
url_code: 'https://github.com/luchengfu6/TextReg'
---

Large language models are highly sensitive to their prompts, and iterative prompt-optimization methods that rewrite prompts from model feedback tend to overfit: prompts grow longer, accumulate narrow sample-specific rules, and generalize poorly beyond the training distribution. We frame this failure mode as **prompt distributional overfitting** and measure it through *representational inefficiency*, which decomposes prompt inefficiency into capacity cost and scope narrowness.

**TextReg** is a regularization framework that realizes a soft-penalty objective through regularized textual gradients, combining three stages: Dual-Evidence Gradient Purification, Semantic Edit Regularization, and Regularization-Guided Prompt Update.

![The TextReg pipeline: Dual-Evidence Gradient Purification, Semantic Edit Regularization, and Regularization-Guided Prompt Update (adapted from the paper).](framework.png)

**My role.** I am a co-author on this collaboration. Across multiple reasoning benchmarks, TextReg substantially improves out-of-distribution generalization, with accuracy gains of up to +11.8% over TextGrad and +16.5% over REVOLVE.
