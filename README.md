# dnaPipelineR-materials

This repository contains **supporting materials** for the dissertation project:
**dnaPipelineR: A Semi-Automated Pipeline for Discourse Network Analysis**.  
It is a companion to the main [dnaPipelineR](https://github.com/sarahtunmore/dnaPipelineR) repository, which contains the runnable R package.

---

## Contents

- **data/**  
  Annotated dataset of 862 statements from UK parliamentary debates, including actor, organisation, concept, and right labels (see dissertation Appendix B for details).

- **experiments/**  
  Scripts and outputs from model training and evaluation, including:
  - Statement segmentation (MLP, embeddings)
  - Concept classification (SVM, MLP, grouped/fine-grained)
  - Right classification (SVM + ablations)
  - Ablation runs (e.g., without POS features)

- **models/**  
  Serialized trained models (`.joblib`) for reproducibility.  
  These are not needed to *run* the pipeline but are included to replicate dissertation experiments.

- **docs/**  
  Notes on experiment settings, results, and reproducibility checklist.

---

## Relationship to Main Repo

- [dnaPipelineR](https://github.com/sarahtunmore/dnaPipelineR):  
  Installable R package for semi-automatic annotation. End users should start here.

- **This repo (`dnaPipelineR-materials`)**:  
  Contains training data, experimental scripts, and supporting materials required for ERP submission and full reproducibility.  
  Not required to run the R package.

---

## Reproducibility

To reproduce experiments:
1. Clone this repo.
2. Navigate into an experiment folder, e.g. `experiments/concept_classification/`.
3. Run the training script (`train_concept.py`) with the provided dataset.  
   Requirements: Python 3.9+, scikit-learn, transformers, joblib.

---

## Citation

If referring to this repository in academic work:

> sarahtunmore (2025). *dnaPipelineR-materials: Supporting materials for ERP dissertation*. GitHub. https://github.com/sarahsorous/dnaPipelineR-materials
