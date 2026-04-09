---
layout: homepage
---

## About Me

- I am a **PhD student** at [MBZUAI](https://mbzuai.ac.ae/), advised by [Alham Fikri Aji](https://scholar.google.com/citations?user=0Cyfqv4AAAAJ&hl=en) and [Yova Kementchedjhieva](https://scholar.google.com/citations?user=Br-FqfIAAAAJ&hl=en). My work focuses on multimodal foundation models, post-training and alignment, grounded vision-language systems, and large-scale evaluation.

- Previously, I was a **Research Engineer** at Singapore Management University, where I worked on multilingual and multimodal interpretation with [Chong-Wah Ngo](https://scholar.google.com/citations?user=HM39HrUAAAAJ&hl=en). Before that, I earned my **B.Eng. in Computer Science** from Institut Teknologi Bandung, where I worked with [Ayu Purwarianti](https://scholar.google.com/citations?user=8jUro_cAAAAJ&hl=en) on synthetic data generation for explainable multimodal reasoning.

- My goal is to build multimodal systems that can properly utilize multimodal evidence and interaction feedback rather than relying on modality-specific shortcuts.

## Research Interests

<div style="margin: 0 0 24px; padding: 18px 22px; border-left: 4px solid #2496cb; background: rgba(36, 150, 203, 0.08); font-style: italic;">
I am interested in creating a multimodal systems that truly perceives all inputs to make grounded judgments and responses, rather than relying on modality-specific shortcuts or shallow priors.
</div>

1. **Modality Utilization.** I study how multimodal models allocate attention and capacity across modalities, and why they often under-utilize informative signals in favor of dominant ones. My work focuses on understanding when and why models fail to fully exploit available modalities, leading to sparse utilization, shortcut learning, hallucination, or language over-reliance. This direction is reflected in the [Synthetic-VQA-NLE](https://arxiv.org/abs/2409.14785) framework, which enables the generation of explainable and sound synthetic VQA data; [SeeingCulture](https://arxiv.org/abs/2509.16517), which diagnoses the lack of domain awareness that distorts visual grounding; and [ConfusedTourists](https://arxiv.org/abs/2511.17004), which points out how perturbing context can trigger biased behavior in grounding systems.

2. **Post-Training on Action-Conditioned Supervision Signals.** To mitigate the above problems, I work on both training and non-training adaptations to improve cross-modal grounding and utilization. My current interests include post-training signals that recover or sharpen modality-specific abilities, distillation, and supervision schemes that could eventually support action-conditioned multimodal systems in which perception, language, and decision-making are tightly coupled. This direction is reflected most directly in [LinguDistill](https://arxiv.org/abs/2604.00829), for its cross-modal distillation attempt to recover the language-centric ability of VLMs, and also connects back to [Synthetic-VQA-NLE](https://arxiv.org/abs/2409.14785) as an earlier step toward better grounded supervision. As you are reading this webpage, I am also actively leading a world model evaluation research to assess plan-action cross-modal consistency, as well as involved in a memory-based VLMs research to boost modality grounding and prevent modality-specific forgetting.

3. **Large-Scale Evaluation.** I also often investigate model robustness under varying resource conditions and modality availability. This involves designing evaluation protocols and infrastructure that probe modality reliance, cross-modal consistency, and broad inclusivity at scale. This direction is reflected in award-winning [WorldCuisine](https://arxiv.org/abs/2410.12705), [SEACrowd](https://arxiv.org/abs/2406.10118) both as a paper and through active organization involvement, [ProxyLM](https://arxiv.org/abs/2406.09334), and [DataRubrics](https://arxiv.org/abs/2506.01789), which together study scalable benchmarking, performance prediction, and data quality assessment.

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
