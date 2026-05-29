---
layout: homepage
---

## About Me

I'm a PhD student at [MBZUAI](https://mbzuai.ac.ae/), advised by [Alham Fikri Aji](https://scholar.google.com/citations?user=0Cyfqv4AAAAJ&hl=en). My work investigates the understanding-generation gap in multimodal models and builds solutions to close it.

Before my PhD, I worked as a Research Engineer at [Singapore Management University](https://www.smu.edu.sg/) with [Chong-Wah Ngo](https://scholar.google.com/citations?user=HM39HrUAAAAJ&hl=en), where I focused on multilingual and multimodal interpretation. I started this path during my Bachelor's in Computer Science at [Institut Teknologi Bandung](https://www.itb.ac.id/), working with [Ayu Purwarianti](https://scholar.google.com/citations?user=8jUro_cAAAAJ&hl=en) on synthetically scaling explainable VQA data.

My goal is to build multimodal systems that perceive, reason, and generate grounded response over complex real-world inputs — not ones that get "lucky" on benchmarks by exploiting shortcuts.

## Research Interests

> *I am interested in understanding the discrepancy between multimodal understanding and generation, and innovating methods to minimize such gap.*

Multimodal models often appear to understand an image well when asked to describe it in dominant modality (e.g. text). But when the same model is asked to use that understanding to generate in non-dominant modality, like images or video, it fails on multiple aspects. My research starts by diagnosing where and why this breakdown happens, then works on the solutions that minimize such discrepancy.

### Understanding
I study how models decide what to attend to, and why they over-rely on language signals while underusing visual inputs. This leads to shortcut learning, hallucination, and weak grounding across different settings — biased visual grounding under semantically-aligned perturbations ([ConfusedTourists](https://arxiv.org/abs/2511.17004)), fragile perceptual attention exposed through counting tasks ([CountingTricks](https://arxiv.org/abs/2604.10039)), and domain gaps that degrade even high-level understanding ([SeeingCulture](https://arxiv.org/abs/2509.16517)), and its reasoning elicitation quality ([Synthetic-VQA-NLE](https://arxiv.org/abs/2409.14785)).

### Generation
These failure modes point toward where to intervene. I work on post-training methods that recover missing abilities and strengthen cross-modal alignment using adaptive distillation. [LinguDistill](https://arxiv.org/abs/2604.00829) shows that language ability degrades during visual training and that distillation can recover it, confirming the gap is real and empirically addressable. On the generation side, I am currently working on world model evaluation for plan-action consistency and memory-based VLMs to achieve better grounding robustness over out-of-distribution data.

### Evaluation
Measuring progress on this gap also requires evaluation setups that are faithful to real-world conditions. I design benchmarks that stress-test model behavior under distribution shifts, missing modalities, and limited resources ([WorldCuisine](https://arxiv.org/abs/2410.12705), [SEACrowd](https://arxiv.org/abs/2406.10118), [DataRubrics](https://arxiv.org/abs/2506.01789)), so that improvements on the generation side can be tracked reliably and at scale.

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
