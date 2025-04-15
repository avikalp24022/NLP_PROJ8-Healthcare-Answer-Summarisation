# NLP_PROJ8-Healthcare-Answer-Summarisation
# INTRO

This repository contains code and experiments related to perspective-aware healthcare answer summarization. The project explores advanced summarization techniques using state-of-the-art language models to generate concise and semantically accurate summaries from healthcare question-answer data.

# Overview

The goal of this project is to develop a summarization model that distills complex, multi-perspective healthcare data into coherent summaries. We investigate various approaches, including zero-shot setups with benchmark models, replication of the PLASMA model, standard fine-tuning of BART Large-CNN and Flan-T5, and a Mixture-of-Experts (MoE) architecture that leverages both Flan-T5 and its LoRA-enhanced variant.

# Data (about PUMA Dataset)

The PUMA dataset is specifically curated for healthcare question-answering tasks. Each entry includes a unique identifier, the question, additional context, a list of answers, labelled answer spans, and labelled summaries corresponding to various perspectives (e.g., INFORMATION, SUGGESTION, CAUSE, and EXPERIENCE), along with the complete raw text. The dataset is divided into training, validation, and testing subsets, which enables a robust evaluation framework for the perspective-aware summarization models.

# Tried Models and Architecture

- **Benchmark Models:**
  - DeepSeek (Zero-shot)
  - BART (Zero-shot)

- **Replicated Architecture:**
  - PLASMA: Perspective-aware summarization model as proposed in the literature

- **Fine-tuning Approaches:**
  - BART Large-CNN: Fine-tuned on the healthcare dataset
  - Flan-T5: Fine-tuned using standard fine-tuning methods

- **Mixture of Experts (MoE):**
  - Flan-T5: Fine-tuned separately for each perspective
  - Flan-T5 with length constraints: Fine-tuned separately for each perspective
  - Flan-T5 with LoRA: A parameter-efficient variant fine-tuned using Low-Rank Adaptation

# Repo Structure
- Baseline Folder : Contians replicated PLASMA Archoitecture codes.
- Structured Fine Tuning : Contains ipynb file for BART and Flan-T5 fine-tuning with generated summaries in csv format.
- MoE : Contains ipyns file for Mixture of Experts Architecture with Flan-T5 as base model with generated summaries in csv format.

# Model Links

- **Standard Fine-Tuning Models:** [Google Drive Folder](https://drive.google.com/drive/folders/12cpzJ7s8Dvhj2-WAY8YO190hq9NCRuXu?usp=sharing)
- **Baselines:** [Google Drive Folder](https://drive.google.com/drive/folders/1wzgfc7164URTYibykmKrXzlKFN0Quv0n?usp=sharing)
- **MoE Saved Models:** [Google Drive Folder](https://drive.google.com/drive/folders/1wzgfc7164URTYibykmKrXzlKFN0Quv0n?usp=sharing)

# Authors

- MT24139 : Shubhankar Tiwary
- MT24078 : Sai Krishna Kota
- MT24022 : Avikalp Rewatkar
