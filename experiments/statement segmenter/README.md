## Overview

These notebooks contain experiments for the statement segmentation task, which identifies whether a text span is a statement (claim) or not.

## Model Variants

- MLP with paraphrase-multilingual-mpnet-base-v2 embeddings

- MLP with all-MiniLM-L6-v2 embeddings

## Key Findings

Both models achieved accuracy ≈ 0.86 with balanced precision/recall.

Paraphrase-multilingual model prioritised recall (0.90), producing more false positives.

all-MiniLM-L6 model had slightly higher precision (0.84 vs. 0.83) but lower recall (0.88 vs. 0.90).

Error analysis showed false positives were often borderline evaluative clauses.

## Reproducibility

Use the balanced dataset (512_each_statements_nonstatements_chunks.xlsx).

Run the notebook sequentially to train and evaluate both embeddings.

Outputs include cross-validation metrics and confusion matrices.
