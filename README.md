# **Image Captioning Models with ResNet50+LSTM, ViT+BERT, and ViT+GPT2**

This repository contains the implementation of three advanced image captioning models:
1. **ResNet50 + LSTM**: A classic approach using Convolutional Neural Networks (CNNs) for image encoding and LSTMs for sequential caption generation.
2. **Vision Transformer (ViT) + BERT**: A transformer-based approach leveraging Vision Transformers (ViT) for image encoding and BERT for text generation.
3. **Vision Transformer (ViT) + GPT2**: A generative model combining ViT for image encoding with GPT2’s autoregressive capabilities for text generation.

Each model integrates a robust visual encoder and a natural language processing decoder to generate descriptive captions for input images.

---

## **Hyperparameters**

The following table summarizes the key training configurations used for each model:

| **Parameter**    | **ResNet50 + LSTM** | **ViT + BERT**  | **ViT + GPT2**  |
|-------------------|---------------------|-----------------|-----------------|
| **Epochs**       | 10                  | 10              | 10              |
| **Batch Size**    | 128                 | 32              | 32              |
| **Learning Rate** | 0.0001              | 0.00001         | 0.00001         |
| **Optimizer**     | Adam                | Adam            | Adam            |
| **Scheduler**     | N/A                 | OneCycleLR      | OneCycleLR      |

---

## **Evaluation Results**

The models were evaluated using popular metrics for image captioning: **BLEU (1-4)**, **METEOR**, and **ROUGE-L**. The table below provides the performance scores for each model:

| **Model**         | **BLEU-1** | **BLEU-2** | **BLEU-3** | **BLEU-4** | **METEOR** | **ROUGE-L** |
|--------------------|------------|------------|------------|------------|------------|-------------|
| **ResNet50 + LSTM**| 0.648      | 0.451      | 0.300      | 0.202      | 0.421      | 0.506       |
| **ViT + BERT**     | 0.725      | **0.551**  | **0.395**  | **0.278**  | 0.501      | **0.546**   |
| **ViT + GPT2**     | **0.728**  | 0.545      | 0.385      | 0.265      | **0.502**  | 0.532       |

---
