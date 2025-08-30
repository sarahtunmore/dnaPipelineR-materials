## Overview

This notebook contains the final implementation of the concept classification task, using a linear SVM on SBERT embeddings.

## Model Variants

- Baseline SVM with embeddings only

- SVM + POS features (concatenating POS-tag distributions to embeddings)


## Key Findings

Baseline SVM achieved Top-1 accuracy of 0.35 with macro precision 0.39, recall 0.30, and F1 0.32.

When allowing Top-3 predictions, accuracy rose to 0.65, demonstrating the value of semi-automatic workflows where annotators can choose among candidate labels.

Adding POS features slightly degraded macro recall and F1, confirming limited usefulness.

## Reproducibility

Load SBERT embeddings for statements (paraphrase-multilingual-mpnet-base-v2).

Train and evaluate the SVM using the provided split.

Compare performance with/without POS-tag features.
