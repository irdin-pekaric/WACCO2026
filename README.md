# [Topical Shifts in the Dark Web: A Longitudinal Analysis of Content in Cybercrime Forums and Marketplaces]

This repository contains the anonymized artifacts accompanying a submission to **WACCO 2026**.

## Overview

This repository provides all scripts and notebooks required to reproduce the data processing, topic modeling, and analysis conducted in the paper. The workflow covers text extraction, preprocessing, multiple topic modeling approaches, and evaluation across several research questions.

All materials are anonymized for the double-blind review process.

---

## Repository Structure

### 📁 data_processing/

This folder contains all preprocessing and data preparation steps.

- **extract_text_from_html.ipynb**  
  Extracts raw textual data from HTML sources.

- **preprocessing_topic_modeling.ipynb**  
  Performs cleaning and normalization tailored for topic modeling.

- **preprocessed_text.ipynb**  
  Handles preprocessing of the original dataset.

- **preprocessed_text_english.ipynb**  
  Processes and prepares English-translated text for analysis.

---

### 📁 topic_modeling/

This folder contains different topic modeling approaches explored in the paper.

- **topic_model_all-MiniLM-L6-v2-loop-openai.ipynb**  
  Topic modeling pipeline using MiniLM embeddings combined with OpenAI-based refinement.

- **topic_model_attack_bert.ipynb**  
  Topic modeling using an AttackBERT-based embedding model.

- **topic_model_dark_bert.ipynb**  
  Topic modeling using DarkBERT embeddings for domain-specific analysis.

- **topic_model_results.ipynb**  
  Aggregates and visualizes topic modeling outputs.

---

### 📁 wordclouds/

This folder contains generated word cloud visualizations for each topic modeling approach, supporting qualitative interpretation of the extracted topics.

- **MiniLM_OpenAI/**  
  Word clouds generated from the MiniLM + OpenAI topic modeling pipeline.

- **AttackBERT/**  
  Word clouds generated from the AttackBERT-based model.

- **DarkBERT/**  
  Word clouds generated from the DarkBERT-based model.

---

### 📁 research_questions/

This folder contains analyses addressing the research questions defined in the paper.

- **q1.ipynb, q1a.ipynb, q1b.ipynb**  
  Experiments and analyses related to Research Question 1.

- **rq2a.ipynb, rq2b.ipynb, rq2c.ipynb**  
  Experiments and analyses related to Research Question 2.

---

### 📁 analysis/

This folder includes supporting analyses and statistical evaluation.

- **results_stats.ipynb**  
  Computes statistical summaries and evaluation metrics.

- **group_snapshots.ipynb**  
  Provides grouped views and intermediate inspection of results.

---

## Reproducibility

All experiments are implemented as Jupyter notebooks. The typical workflow is:

1. Run preprocessing scripts in `data_processing/`
2. Execute topic modeling notebooks in `topic_modeling/`
3. Review generated word clouds in `wordclouds/`
4. Run research question analyses in `research_questions/`
5. Evaluate results using notebooks in `analysis/`

---

## Notes

- This repository is anonymized for peer review.
- External dependencies (e.g., APIs, pretrained models) are referenced within the notebooks where applicable.
- Paths and data sources may need adjustment depending on the execution environment.

---

## Contact

Contact information will be provided after the review process.
