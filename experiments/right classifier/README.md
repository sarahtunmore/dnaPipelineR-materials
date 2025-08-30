## Overview

This notebook implements the right classification task, where statements are mapped to one of six labour standards (EQUAL, GENERAL, SECURITY, STATUS, STRIKE, WAGES).

## Model Variants

- Baseline SVM with SBERT embeddings

- SVM + POS features (11 normalised POS-tag distributions added to embeddings)

## Key Findings

Overall accuracy = 0.71, with stronger performance on frequent classes (STRIKE, GENERAL).

Rare classes (EQUAL, STATUS) were consistently weak due to limited training data.

POS features provided negligible gains (macro precision rose slightly from 0.54 → 0.55).

## Reproducibility

Load annotated dataset (862 statements).

Train SVM with/without POS-tag features.

Outputs include full per-class breakdown of precision, recall, and F1.
