# SemEval-2026 Polarization Detection – Subtask 1

This repository contains our system for **SemEval 2026 Task 9 – Subtask 1: Polarization Detection**.

The task is a **binary text classification problem** that determines whether a social media post contains **polarized content**.

Although the task is multilingual, **our work focuses only on Bengali (Bangla) posts**.

---

# Task Description

Each text is classified into one of two labels:

* **Polarized (1)** → The text expresses polarized opinions such as hostility, stereotyping, vilification, or strong ideological division.
* **Non-Polarized (0)** → The text does not contain polarized attitudes.

A text should only be labeled **polarized** when it clearly reflects attitude polarization in context.

---

# Dataset

The Bengali dataset released for the task contains **5,000 social media posts**:

| Split | Instances |
| ----- | --------- |
| Train | 3333      |
| Dev   | 166       |
| Test  | 1501      |

Posts are labeled as **polarized (1)** or **non-polarized (0)**.

---

# Methodology (Brief)

We experimented with two types of approaches:

**Transformer-based models**

* Fine-tuned multilingual and Bangla transformer encoders
* Models include **mBERT, XLM-RoBERTa, MuRIL, and BanglaBERT**

**Prompt-tuned LLMs**

* Instruction-tuned LLMs with prompt-based supervision
* Models include **Qwen, LLaMA, Gemma, and Mistral**
* Parameter-efficient fine-tuning was performed using **LoRA**

LLM-based approaches with **Bangla prompts** showed the best performance for detecting nuanced polarization.

---

# Evaluation

Systems are evaluated using **Macro F1-score** between predicted and gold labels.

Our best model achieved:

**Macro F1: 0.8582**
**Rank: 2nd place among 49 teams**

---

# Paper

For full details about experiments and analysis, see the system description paper included in this repository.
