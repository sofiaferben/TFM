# `modelling/results/`

This folder contains all tabular outputs generated during the training and evaluation of machine learning models for drug synergy prediction. Each `.csv` file corresponds to the evaluation metrics of a particular modeling strategy using a specific synergy score (e.g., HSA, ZIP, Bliss, Loewe).

##  Folder Structure and Description

### `cross_validation/`
Contains results from **standard cross-validation** experiments using the full feature set.

Files:
- `hsa_cv.csv`
- `zip_cv.csv`
- `bliss_cv.csv`
- `loewe_cv.csv`

### `nested_crossss_validation/`
Contains results from **nested cross-validation** (NCV) using the full feature set.

Files:
- `hsa_ncv.csv`
- `zip_ncv.csv`
- `bliss_ncv.csv`
- `loewe_ncv.csv`

### `nested_cross_validation_drugs/`
Contains results from nested cross-validation  using drug signature features.

Files:
- `hsa_drugs.csv`
- `zip_drugs.csv`
- `bliss_drugs.csv`
- `loewe_drugs.csv`

### `nested_cross_validation_nm/`
Contains results from nested cross-validation using only Network Medicine features 

Files:
- `hsa_nm.csv`
- `zip_nm.csv`
- `bliss_nm.csv`
- `loewe_nm.csv`

---

Each `.csv` file summarizes performance metrics (e.g., R², MAE, RMSE) for **18 model pipelines**, defined by combinations of algorithms, preprocessing strategies, and feature selectors.
