---
layout: homepage
---

## About Me

I'm a PhD student at [MBZUAI](https://mbzuai.ac.ae/), advised by [Alham Fikri Aji](https://scholar.google.com/citations?user=0Cyfqv4AAAAJ&hl=en). My research studies how multimodal systems can acquire new skills more efficiently through better learning algorithms, adaptive inference, and scalable post-training / training orchestration.


Before joining MBZUAI, I worked as a Research Engineer at [Singapore Management University](https://www.smu.edu.sg/) under [Chong-Wah Ngo](https://scholar.google.com/citations?user=HM39HrUAAAAJ&hl=en) on multilingual and multimodal learning. I completed my Bachelor’s at [Institut Teknologi Bandung](https://www.itb.ac.id/) under [Ayu Purwarianti](https://scholar.google.com/citations?user=8jUro_cAAAAJ&hl=en), where I worked on scalable explainable VQA data generation.

Ultimately, I hope to build multimodal systems that can perceive, reason, act, and more importantly **adapt** in open-world environments.

## Research Interests

<div style="margin: 0 0 24px; padding: 18px 22px; border-left: 4px solid #2496cb; background: rgba(36, 150, 203, 0.08); font-style: italic;">
How can multimodal systems continue learning efficiently after pretraining?
</div>

My research is centered on this question. I am interested in building multimodal systems that can keep improving from data, interaction, and observation, rather than relying only on larger pretraining datasets or brute-force scaling.

### Efficient Multimodal Learning
My research aims to understand how multimodal systems can acquire new capabilities with less data, less supervision, and less compute. I am particularly interested in learning beyond pretraining through post-training, adaptive inference, continual adaptation, and interaction with the environment.

### Adaptive Learning
I study how models can improve after pretraining through post-training, reinforcement learning, test-time scaling, test-time adaptation, and continual learning. This line of work includes [LinguDistill](https://arxiv.org/abs/2604.00829) and emerging efforts around inference-time adaptation and continual improvement.

### Memory & World Models
To support more robust and flexible learning, I am interested in memory-based representations and world models that enable planning, action reasoning, and skill acquisition. This includes work on conditional memory, model-based reasoning, and long-horizon decision making.

### Evaluation
I also develop benchmarks that diagnose where current multimodal systems fail and how progress should be measured. This includes work on [ConfusedTourists](https://arxiv.org/abs/2511.17004), [CountingTricks](https://arxiv.org/abs/2604.10039), [SeeingCulture](https://arxiv.org/abs/2509.16517), [WorldCuisine](https://arxiv.org/abs/2410.12705), [SEACrowd](https://arxiv.org/abs/2406.10118), and related evaluation efforts.

## Updates

- **[Jun. 2026]** Started exploring test-time scaling for multimodal world models and inference-time adaptation.
- **[May. 2026]** Initial experiments on conditional memory for Vision Transformers are underway.
- **[Apr. 2026]** [LinguDistill](https://arxiv.org/abs/2604.00829) is out on arXiv, studying how selective cross-modal distillation can recover linguistic ability in VLMs while preserving multimodal competence 🧠
- **[Feb. 2026]** Two papers accepted to **CVPR 2026**: [M4-RAG](https://arxiv.org/abs/2512.05959) and [Vision Language Models are Confused Tourists](https://arxiv.org/abs/2511.17004) 🎉
- **[Nov. 2025]** Our study on culturally-conflicting visual reasoning, [Vision Language Models are Confused Tourists](https://arxiv.org/abs/2511.17004), is now on arXiv 🧳
- **[Oct. 2025]** [Entropy2Vec](https://arxiv.org/abs/2509.05060) got accepted into **MRL Workshop @ EMNLP 2025** 🌐🇨🇳
- **[Jul. 2025]** [Seeing Culture Benchmark](https://seeingculture-benchmark.github.io/) is accepted to **EMNLP 2025** 🇨🇳
- **[Apr. 2025]** [WorldCuisines](https://worldcuisines.github.io/) receives **Best Theme Paper** at **NAACL 2025** 🎉🌏🍽️
- **[Mar. 2025]** Admitted to the Fall 2025 cohort of the **MBZUAI PhD program in NLP** 📚
- **[Jan. 2025]** [WorldCuisines](https://worldcuisines.github.io/) and [ProxyLM](https://github.com/davidanugraha/proxylm) are accepted to **NAACL 2025** 🇺🇸🎖️

{% include_relative _includes/publications.md %}

{% include_relative _includes/services.md %}
