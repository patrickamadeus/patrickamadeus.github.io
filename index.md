---
layout: homepage
---

## About Me

- I am a **PhD student** at [MBZUAI](https://mbzuai.ac.ae/), advised by [Alham Fikri Aji](https://scholar.google.com/citations?user=0Cyfqv4AAAAJ&hl=en) and [Yova Kementchedjhieva](https://scholar.google.com/citations?user=Br-FqfIAAAAJ&hl=en). My work focuses on multimodal learning, post-training and alignment, grounded vision-language systems, and large-scale evaluation.

- Previously, I was a **Research Engineer** at Singapore Management University, where I worked on multilingual and multimodal interpretation with [Chong-Wah Ngo](https://scholar.google.com/citations?user=HM39HrUAAAAJ&hl=en). Before that, I earned my **B.Eng. in Computer Science** from Institut Teknologi Bandung, where I worked with [Ayu Purwarianti](https://scholar.google.com/citations?user=8jUro_cAAAAJ&hl=en) on synthetic data generation for explainable multimodal reasoning.

- I further aim to build multimodal systems that reason
effectively across diverse perceptual / action-based inputs without relying on modality-specific shortcuts.

## Research Interests

<div style="margin: 0 0 24px; padding: 18px 22px; border-left: 4px solid #2496cb; background: rgba(36, 150, 203, 0.08); font-style: italic;">
I am interested in building multimodal systems that reasonably leverage its perceptual & semantic inputs to make grounded decisions and responses, rather than relying on shortcuts from a single modality.
</div>

1. **Modality Utilization.**  
    I study how multimodal models decide what to attend to, and why they often rely on dominant signals (e.g., language) instead of fully using other multimodal inputs. This leads to shortcut learning, hallucination, and weak grounding.  
    - [Synthetic-VQA-NLE](https://arxiv.org/abs/2409.14785): synthetic explainable VQA generation pipeline, evaluates VQA reasoning of SOTA VLMs (at the time)
    - [SeeingCulture](https://arxiv.org/abs/2509.16517): shows how lack of domain awareness harms visual grounding and segmentation ability
    - [ConfusedTourists](https://arxiv.org/abs/2511.17004): evaluates how semantically-aligned perturbation context changes trigger biased visual grounding
    - [CountingTricks](https://arxiv.org/abs/2604.10039): exposes straightforward perceptual counting ability of VLMs and how attention-balancing RL post-training may help mitigate this

2. **Post-Training & Cross-Modal Alignment.**  
    To address these issues, I work on post-training methods that improve how models use and connect modalities, including distillation and dynamic supervision signals (action-conditioned signals, RL). The goal is to recover missing abilities and strengthen cross-modal alignment.  
    - [LinguDistill](https://arxiv.org/abs/2604.00829): uses cross-modal distillation to recover degraded language abilities in VLMs  
    - [Synthetic-VQA-NLE](https://arxiv.org/abs/2409.14785): also supports more grounded supervision signals  
    - Ongoing: world model evaluation for plan–action consistency, and memory-based VLMs to improve long-term grounding  

3. **Large-Scale Evaluation.**  
    I also keen on being critical at designing faithful large-scale evaluation setups to understand how models behave under distribution shifts, missing modalities, or limited resources, with focus on reliability and robustness at scale.
    - [WorldCuisine](https://arxiv.org/abs/2410.12705): benchmarks domains-specific cultural and multilingual reasoning in VQA
    - [SEACrowd](https://arxiv.org/abs/2406.10118): builds large-scale multimodal datasets hub for underrepresented languages in 4+ modality mixtures
    - [ProxyLM](https://arxiv.org/abs/2406.09334): efficient multilingual performance prediction system leveraging data and language features
    - [DataRubrics](https://arxiv.org/abs/2506.01789): studies data quality and faithful benchmark creation aspects

## Updates

- **[Apr. 2026]** [LinguDistill](https://arxiv.org/abs/2604.00829) is out on arXiv. We study how selective cross-modal distillation can recover linguistic ability in VLMs while preserving multimodal competence 🧠
- **[Feb. 2026]** 2 papers accepted to **CVPR 2026**! [M4-RAG](https://arxiv.org/abs/2512.05959) gets in as a main paper, and [Vision Language Models are Confused Tourists](https://arxiv.org/abs/2511.17004) appears in findings 🎉
- **[Nov. 2025]** Our study exposing the confusion of VLMs in cultural-conflict visual scenarios, [Vision Language Models are Confused Tourists](https://arxiv.org/abs/2511.17004), is up on arXiv 🧳
- **[Dec. 2025]** [M4-RAG](https://arxiv.org/abs/2512.05959) is out on arXiv! We present an evaluation of how multimodal knowledge enrichment helps models tackle multilingual queries. Spoiler: it does not always help... 🤯
- **[Oct. 2025]** [Entropy2Vec](https://arxiv.org/abs/2509.05060) got accepted into **MRL Workshop @ EMNLP 2025** 🌐🇨🇳
- **[July 2025]** [Seeing Culture Benchmark](https://seeingculture-benchmark.github.io/) is accepted to **EMNLP 2025** 🇨🇳 On to the next one with the SMU Multimedia team 💪
- **[May. 2025]** [DataRubrics](https://arxiv.org/abs/2506.01789) is now on arXiv! We propose a unified scorecard to evaluate data quality on multi-faceted metrics 📊
- **[Apr. 2025]** [WorldCuisines](https://worldcuisines.github.io/) receives **Best Theme Paper** at **NAACL 2025** 🎉🌏🍽️
- **[Mar. 2025]** Admitted to the Fall 2025 cohort of the **MBZUAI PhD program in NLP** 📚
- **[Jan. 2025]** [WorldCuisines](https://worldcuisines.github.io/) and [ProxyLM](https://github.com/davidanugraha/proxylm) are accepted to **NAACL 2025** 🇺🇸🎖️
- **[Nov. 2024]** My first first-author paper, [Towards Efficient and Robust VQA-NLE Data Generation with Large Vision-Language Models](https://arxiv.org/abs/2409.14785), is accepted to **COLING 2025** 🎉
- **[Oct. 2024]** [WorldCuisines](https://worldcuisines.github.io/), the largest multicultural VL food benchmark, is released. Honored to co-lead the project 🥘
- **[Sep. 2024]** [SEACrowd](https://arxiv.org/abs/2406.10118) is accepted to **EMNLP 2024** 🇺🇸

{% include_relative _includes/publications.md %}

{% include_relative _includes/services.md %}
