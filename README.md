# SemEval-2026 – Polarization Detection (Subtask 1)

This repository contains our implementation for **Subtask 1: Polarization Detection** from **SemEval 2026 Task 9 – *Multilingual Text Classification Challenge*.

## Task Description

The objective of this subtask is to perform **binary classification** to determine whether a given post contains **polarized content**.

### Labels

* **Polarized (True = 1)** → The text expresses a polarized opinion or strong ideological stance.
* **Non-Polarized (False = 0)** → The text does not contain polarized opinion.

A text should only be labeled **polarized** when it clearly reflects attitude polarization. If the text does not display such characteristics, it should be labeled **non-polarized**. The overall context and meaning of the text should be considered rather than isolated words.

## Dataset

The organizers provide a **training dataset with labels** for model development.
The task involves **multilingual social media text**.

## Evaluation

Submissions are evaluated using **Macro F1-score**, computed between the predicted labels and the gold labels
