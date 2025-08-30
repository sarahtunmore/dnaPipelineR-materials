# Experiments

This folder contains all experimental notebooks developed as part of the MSc Extended Research Project.
Each notebook records the training, evaluation, and ablation experiments that informed the final models integrated into the dnaPipelineR pipeline.

All code was run in Google Colab to leverage GPU/TPU resources. The notebooks were then downloaded as .ipynb files and uploaded here so that results and outputs can be viewed directly in GitHub without re-running the code.

## Contents

- experiments_for_concept_classifier.ipynb
  Exploratory experiments for concept classification, including SVMs, MLPs, cosine similarity baselines, class weighting, and POS-tag features.

- SVM_for_concept_classification.ipynb
Final linear SVM implementation for concept classification. Tested with and without POS-tag features.

- SVM_for_right_classification.ipynb
SVM models for right classification (6 categories), with experiments on including POS-tag features.

- paraphrase_multilingual_MLP_for_statement_segmentation.ipynb
MLP statement segmentation using paraphrase-multilingual-mpnet-base-v2 embeddings.

- all_MiniLM_L6_MLP_for_statement_segmentation.ipynb
MLP statement segmentation using all-MiniLM-L6-v2 embeddings.

## Notes on Reproducibility

The notebooks are fully executable and can be re-run in Colab or Jupyter using the datasets in the data/ folder.

Because outputs are preserved in the .ipynb files, you can view results directly (tables, confusion matrices, metrics) without re-running the code.

For detailed interpretation of results, see the corresponding sections in the dissertation.
