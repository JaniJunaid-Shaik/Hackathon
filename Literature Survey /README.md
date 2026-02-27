# Literature Survey

This section reviews the foundational and state-of-the-art research papers that support the design and implementation of our **AI-Based Phishing Email Detection System using NLP, Transformers, and LLM Explainability**.

Our system follows a hybrid pipeline combining classical NLP, modern Transformer models, and explainable AI. The research papers below provide theoretical foundations, architectural inspiration, and practical justification for each stage of the pipeline. :contentReference[oaicite:0]{index=0}

---

# 1. Attention Is All You Need  
**Authors:** Vaswani et al., 2017  
**Link:** https://arxiv.org/abs/1706.03762  

---

## Summary

This paper introduced the **Transformer architecture**, which replaced traditional RNN and CNN models with a system based entirely on **self-attention mechanisms**.

Instead of processing words sequentially, the Transformer allows every word in a sentence to attend to every other word simultaneously.

Key contributions:

- Introduced **Self-Attention**
- Introduced **Multi-Head Attention**
- Enabled parallel processing of text
- Improved accuracy and training efficiency

The paper states that the Transformer can capture dependencies regardless of distance between words, making it highly effective for language understanding. :contentReference[oaicite:1]{index=1}

---

## How this helps our project

This paper forms the **core foundation of the Transformer stage** in our phishing detection pipeline.

Specifically, it enables:

- Understanding contextual meaning of email text
- Detecting phishing intent even when obvious keywords are absent
- Identifying relationships between words like:

Example:

> "Verify your account immediately"

Transformer understands urgency + intent.

Without this paper, modern phishing detection using Transformers would not exist.

---

# 2. BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding  
**Authors:** Devlin et al., 2019  
**Link:** https://arxiv.org/abs/1810.04805  

---

## Summary

This paper introduced **BERT**, a Transformer-based model that understands language using **bidirectional context**.

Unlike previous models that read text in one direction, BERT reads text:

Left → Right  
Right → Left  

simultaneously.

This allows deeper understanding of meaning.

The paper explains that BERT uses:

- Masked Language Modeling
- Next Sentence Prediction

to learn language patterns. :contentReference[oaicite:2]{index=2}

BERT achieved state-of-the-art performance on multiple NLP tasks.

---

## How this helps our project

This paper directly supports the **Transformer classification stage** of our phishing detection system.

BERT helps detect:

- Subtle phishing intent
- Context-based manipulation
- AI-generated phishing emails

Example:

Email:

> "Due to policy changes, confirm access"

Traditional model: unsure

BERT: identifies phishing intent clearly

This improves:

- Accuracy
- Context understanding
- Detection reliability

---

# 3. On the Space-Time Expressivity of ResNets  
**Author:** Müller, 2020  
**Link:** https://arxiv.org/abs/1910.09599  

---

## Summary

This paper explains how **Residual Neural Networks (ResNets)** can approximate highly complex patterns.

ResNets use:

Skip connections: x(k+1) = x(k) + R(x(k))


This helps:

- Improve learning stability
- Prevent vanishing gradient problem
- Enable deep model training

The paper proves ResNets can approximate complex functions with high accuracy. :contentReference[oaicite:3]{index=3}

---

## How this helps our project

This paper supports the **deep learning reliability and stability** of our system.

It explains why deep architectures like:

- BERT
- Transformer
- Neural classifiers

can learn complex phishing patterns.

This strengthens confidence in using deep models.

---

# 4. Attentional Prototype Inference for Few-Shot Segmentation  
**Authors:** Sun et al., 2023  
**Link:** https://arxiv.org/abs/2105.06668  

---

## Summary

This paper introduces a system that combines:

- Attention mechanisms
- Probabilistic modeling
- Prototype-based learning

to improve classification accuracy under uncertainty.

It models data as distributions instead of fixed values.

This improves:

- Robustness
- Generalization
- Accuracy

The paper states probabilistic attention helps models handle uncertainty and variations effectively. :contentReference[oaicite:4]{index=4}

---

## How this helps our project

This paper supports the **confidence scoring and robustness** of our phishing detection system.

It helps justify:

- Confidence score output
- Better generalization to new phishing attacks
- Improved reliability

This improves real-world usability.

---

# Overall Contribution to Our Project

These four papers collectively support the full pipeline of our system:

| Pipeline Stage | Supporting Paper |
|---|---|
| NLP Understanding | BERT |
| Transformer Classification | Attention Is All You Need |
| Deep Learning Stability | ResNet Expressivity |
| Confidence & Robustness | Attentional Prototype Inference |

---

# Conclusion

The literature strongly supports using a hybrid architecture combining:

- NLP preprocessing
- Transformer classification
- Deep learning models
- Explainable AI

These research works validate our approach and provide a strong scientific foundation for building an accurate and reliable phishing email detection system.


