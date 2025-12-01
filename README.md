# Self-Empowering VLMs: Achieving Hierarchical Consistency via Self-Elicited Knowledge Distillation

Official implementation of  
**"Self-Empowering VLMs: Achieving Hierarchical Consistency via Self-Elicited Knowledge Distillation"**  
by **Wei Yang\*, Yiran Zhu\*, Zilin Li, Xunjia Zhang, Hongtao Wang†**  

\* Co-first authors &nbsp;&nbsp; † Corresponding author

- 📝 Paper: [arXiv PDF](https://arxiv.org/pdf/2511.18415.pdf)  
- 🌐 Project page: https://ciaranz.github.io/SEKD.github.io/  

---

## 🔍 Overview

Vision-language models (VLMs) contain rich taxonomic knowledge, but often fail on **hierarchical visual question answering (VQA)**, where predictions must stay consistent along a **coarse-to-fine label path**.

In this work, we

- analyze several inference paradigms for hierarchical VQA;
- show that **step-wise conditioning on previous answers** is highly effective;
- identify that the main bottleneck is **maintaining cross-level state**, rather than recalling labels;
- propose **Self-Empowering Knowledge Distillation (SEKD)**:
  - a multi-step teacher VLM supervises a single-pass student,
  - using hard labels, soft distributions, and hidden states.

SEKD yields

- significantly improved **hierarchical consistency** on both in-domain and **zero-shot** taxonomies;
- better performance on **challenging mathematical reasoning** benchmarks;
- without requiring any **extra human annotations**.

