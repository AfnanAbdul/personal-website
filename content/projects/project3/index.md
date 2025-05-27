---
title: "Detecting AI-Generated Text: Targeting Academic Integrity Applications"
date: 2025-05-26
lastmod: 2025-05-26
tags: ["LLMs", "AI Text Detection", "RoBERTa", "LoRA", "RAID", "Academic Integrity", "Transformers", "Binary Classification", "Python", "PyTorch", "HuggingFace", "RAID Dataset"]
description: "Developed a robust AI text detection model focused on minimizing false positives in academic writing using RoBERTa with parameter-efficient fine-tuning."
summary: "Completed for DS6051: Decoding Large Language Models at UVA, this project explores transformer-based methods for detecting AI-generated text in academic contexts. By fine-tuning RoBERTa using LoRA and optimizing for human accuracy, the model reduced false positives on human-written abstracts from 83.2% to just 0.7%, demonstrating the importance of fairness and robustness in detection systems."
showToc: false
showToc: false
weight: 3
cover:
    image: "project3.png"
    alt: "AI-Generated Text Detection"
    relative: false
---

---

##### Links

+ [Paper](DS6051_Final_Report.pdf)
+ [Code](https://github.com/AfnanAbdul/TuringLens)
+ [Presentation Slides](AI_Detection_Presentation.pdf)

---

##### Overview

Developed a transformer-based AI text detection model to distinguish between human and AI-generated academic writing, specifically engineered to address false positive bias in academic settings where students' legitimate work was being wrongly flagged as AI-generated. Using RoBERTa with LoRA (Low-Rank Adaptation), achieved 99.6% accuracy while requiring only 0.82% trainable parameters compared to full fine-tuning approaches. Implemented a two-stage training methodology: initially trained on ~1,378 essays from Kaggle, then evaluated and fine-tuned on academic abstracts from the RAID dataset including adversarial examples designed to evade detection. Focused on minimizing unfair misclassification of real student work by applying aggressive 10:1 class weighting and optimizing for fairness-focused metrics like human accuracy and balanced accuracy, reducing false positives on human academic writing from 83.2% to 0.7% while maintaining 99.4% AI detection accuracy.

---

##### Next Steps

Building on our initial detection framework, I plan to continue this research independently to further explore the extent to which LLM-generated content can be effectively detected and contribute to the broader discussion on ethical AI usage in education.

**Enhanced Detection Methods and Benchmarking**
- Conduct thorough analysis of existing detection models and methods, expanding beyond our initial three-model comparison to include state-of-the-art approaches and commercial tools
- Implement the stylometric features identified in our future work, including perplexity and burstiness analysis, vocabulary richness metrics, and sentence complexity measurements to create more sophisticated hybrid detection models
- Explore integration of traditional linguistic features with our transformer-based approach to improve robustness and generalizability

**Comprehensive RAID Dataset Evaluation**
- Expand evaluation to the complete RAID test dataset beyond our focused subset of academic abstracts, testing across all domains including news articles, creative writing, technical documentation, and social media content
- Submit results to the RAID leaderboard to benchmark our approach against other state-of-the-art detection methods and establish comparative performance metrics
- Analyze performance variations across different text domains and LLM source models to understand generalization capabilities

**Robustness and Real-World Application**
- Evaluate detection performance against newer and evolving LLM architectures to ensure sustained effectiveness as AI text generation continues to advance
- Investigate adversarial robustness by testing against AI-generated content specifically designed to evade detection systems
- Develop practical implementation tools including web interfaces or API endpoints that educators could integrate into existing academic workflows

**Ethical AI and Academic Integrity**
- Conduct comprehensive fairness audits to ensure equitable performance across diverse student populations and writing styles, addressing potential biases in detection accuracy
- Implement explainable AI features to help educators understand detection decisions and support more informed academic integrity assessments
- Explore confidence scoring mechanisms that provide nuanced predictions rather than binary classifications, better serving real-world educational decision-making

---

#### Related material

+ [OpenAI ends its AI text classifier due to low accuracy (TechCrunch)](https://techcrunch.com/2023/07/25/openai-scuttles-ai-written-text-detector-over-low-rate-of-accuracy/)
+ [Texas A&M professor falsely accuses class of using ChatGPT (Rolling Stone)](https://www.rollingstone.com/culture/culture-features/texas-am-chatgpt-ai-professor-flunks-students-false-claims-1234736601/)

