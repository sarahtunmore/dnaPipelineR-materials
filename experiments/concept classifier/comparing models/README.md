## Overview

This notebook contains exploratory experiments for the concept classification task in the dnaPipelineR pipeline. The aim was to test a variety of machine learning architectures for mapping statements to 21 fine-grained concept categories in the labour-law codebook.

Experiments Included

- Support Vector Machine (SVM) with SBERT embeddings

- Multilayer Perceptron (MLP) with SBERT embeddings

- Cosine similarity with seed sentences (baseline)

- SVM with class weighting (to mitigate rare-class imbalance)

- SVM with engineered features (POS-tag frequencies appended to embeddings)

## Key Findings

All models struggled with rare categories, reflecting the long-tailed distribution of the dataset.

MLPs achieved higher overall accuracy than SVMs but were unstable across folds, collapsing on rare categories.

The linear SVM proved more reliable under data scarcity and was adopted as the final model.

POS-tag features provided negligible improvements.


## Reproducibility

To re-run the experiments:

Load MANUALLY_ANNOTATED_DATA.xlsx from the data/ folder.

Run cells in sequence; models output metrics (accuracy, macro/weighted P/R/F1).

Detailed results are logged inline with the notebook outputs.
