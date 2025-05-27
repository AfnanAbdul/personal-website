---
title: "Comparative Study of Large Language Model Evaluation Frameworks"
date: 2025-05-23
lastmod: 2025-05-23
tags: ["LLMs", "LLM-as-a-Judge","AI Ethics", "Bias Detection", "Model Evaluation", "Python", "Claude", "RAGAS", "promptfoo", "DeepEval", "TruLens", "UVA", "Data Science Capstone"]
description: "A comprehensive analysis of evaluation frameworks for LLMs, focusing on bias detection, response quality, and robustness."
summary: "As part of my capstone project for the M.S. in Data Science at the University of Virginia in collaboration with Deloitte, this research critically examines leading frameworks for evaluating large language models (LLMs). The study leverages multiple datasets and methodologies to benchmark state-of-the-art approaches for ethical and reliable AI assessment. This comprehensive research systematically evaluated and compared multiple LLM evaluation frameworks across eight critical metrics: toxicity detection, bias detection, hallucination detection, summarization quality, tone identification, readability assessment, retrieval accuracy, and response accuracy."
showToc: false
weight: 1
cover:
    image: "project1.png" 
    alt: "LLM Evaluation Framework Comparison"
    relative: false
---

---

##### Links

+ [Paper](LLM_as_a_judge_Deloitte.pdf)
+ [Code](https://github.com/AfnanAbdul/LLM-eval-framework-comparison)
+ [Presentation Slides](1003am_deloitte_anthropic_llm.pdf)
+ [LLM Evaluation Framework Leaderboard](https://llm-evaluation-framework-leaderboard.vercel.app)

---

##### Overview

As part of my UVA capstone project, I collaborated with an industry sponsor to analyze and compare evaluation frameworks for large language models (LLMs). This study focused on key metrics such as response accuracy, retrieval effectiveness, bias detection, toxicity, hallucination, and tone identification. I led the bias detection evaluation, implementing Counterfactual Data Testing with the WinoBias dataset to measure LLM response consistency across sensitive attributes. Additionally, I developed and applied custom bias detection methods using promptfoo, DeepEval, and RAGAS, conducting comparative analyses on 1,500+ sentence pairs from the CrowS-Pairs dataset. By integrating counterfactual data testing with contextual sensitivity analysis, our research aimed to enhance gender bias evaluation in LLMs and contribute to more ethical AI assessment methodologies.

---

#### Related material

+ [🏛️ UVA Master’s in Data Science Students Showcase Real-World Solutions in 2025 Capstone Presentations](https://bit.ly/3RTDgCo)
