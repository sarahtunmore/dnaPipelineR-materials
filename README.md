# dnaPipelineR-materials

This repository contains **supporting materials** for the MSc Extended Research Project:
**Developing a Semi-Supervised Text Annotation Pipeline for Political Discourse Analysis using Natural Language Processing and Machine Learning Techniques**.  

It complements the main [dnaPipelineR](https://github.com/sarahtunmore/dnaPipelineR) repository, which provides the usable R package implementation of the final pipeline.
This repository provides the datasets, experimental notebooks, and documentation required for reproducibility and transparency.

---

# Repository Structure

## data/

- `MANUALLY_ANNOTATED_DATA.xlsx` – Full annotated dataset (862 statements).

- `512_each_statements_nonstatements_chunks.xlsx` – Balanced dataset for statement segmentation (512 statements, 512 non-statements).

- `metadata.docx` – Full description of the datasets, annotation process, variables, ethics/licensing, and Hansard sources.

- (Codebook available in dissertation appendix; may be added here if approved.)

## experiments/
Jupyter notebooks documenting all experiments for concept classification, right classification, and statement segmentation.

- Exploratory and ablation experiments (`experiments_for_concept_classifier.ipynb`).

- Final SVM implementations for concepts and rights (`SVM_for_concept_classification.ipynb`, `SVM_for_right_classification.ipynb`).

- Statement segmentation models using multilingual and MiniLM embeddings (`paraphrase_multilingual_MLP_for_statement_segmentation.ipynb`, `all_MiniLM_L6_MLP_for_statement_segmentation.ipynb`).

- All code was run in Google Colab for processing power and exported as .ipynb so outputs can be viewed directly without re-running.

# How to Use
1) Datasets – Found in data/. These can be loaded directly into Python, R, or DNA software for replication.

2) Notebooks – Open any .ipynb in GitHub to view results (metrics, confusion matrices, error analysis). To re-run: download the notebook and open in Google Colab or Jupyter.

3) Pipeline – The runnable pipeline is provided in the dnaPipelineR repository.

---

# Citation

If referring to this repository in academic work:

> sarahtunmore (2025). *dnaPipelineR-materials: Supporting materials for ERP dissertation*. GitHub. https://github.com/sarahsorous/dnaPipelineR-materials
