#  `code/` – Modeling Scripts

This folder contains all the Jupyter notebooks used to train and evaluate models for drug synergy prediction across different synergy scoring strategies.

##  Structure and Purpose

Each notebook corresponds to a specific **training strategy**, trained with a specific ** HSA synergy score** (all the possible types are HSA, ZIP, Bliss, Loewe). All notebooks are designed to be run independently and follow a consistent structure, allowing for easy comparison of modeling results across scoring approaches.


##  Notebook Descriptions

- `1_cross_validation_hsa.ipynb`  
  Baseline cross-validation (non-nested) for HSA synergy score.

- `2_nested_cross_validation_hsa.ipynb`  
  Full nested cross-validation pipeline for HSA, evaluating all 18 model configurations.

- `3_nested_cross_validation_drugs_hsa.ipynb`  
  Nested CV on the same HSA dataset, but designed to split train/test by drug identity (for out-of-distribution testing on unseen drugs).

- `4_nested_cross_validation_nm_hsa.ipynb`  
  Nested CV using HSA but focused on the **Network Medicine** subset of features, providing insights into the added value of interactome-derived variables.

##  Modeling Strategy

Across all notebooks, the core idea is to evaluate **18 distinct ML pipelines**, varying in:
- Model type (e.g., XGBoost, CatBoost, Random Forest, etc.)
- Preprocessing steps (e.g., normalization, scaling)
- Feature selection strategy (e.g., univariate filtering, recursive elimination)

This enables robust benchmarking and allows us to determine which combinations are most predictive for each synergy score definition.

## How to Run

1. Open the desired notebook for a specific strategy.
2. Change the synergy score determined
4. Run all cells sequentially.
5. Outputs (e.g., results CSV, trained model objects, plots) will be saved to the corresponding `results/` and `figures/` directories.

