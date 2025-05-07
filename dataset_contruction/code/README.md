## /code - Dataset Construction Scripts

This folder contains Jupyter notebooks used in the construction and processing of the dataset for the Master's Thesis project.Each script is numbered to reflect the intended order of execution, ensuring a clear and reproducible data processing pipeline.

---

##  Contents

| File Name            | Description                                                   |
|---------------------|---------------------------------------------------------------|
| `1_drugcombdb.ipynb` | Notebook for loading and exploring the DrugCombDB dataset.   |
| `2_drugcomb.ipynb`   | Notebook for loading and exploring the DrugComb dataset      |
| `3_therapeutic_data_commons.ipynb`   | Notebook for loading and exploring the Therapeutic Data Commons dataset      |
| `4_synergxdb.ipynb`   | Notebook for loading and exploring the SynergxDB dataset      |
| `5_cmaps.ipynb`   | Notebook for processing CMAP/L1000 data      |
| `6_drugcomb_cmap.ipynb`   | Notebook for merging DrugComb & CMAP signatures     |
| `7_vae_data_preparation.ipynb`   | Notebook for preparing drug signature data to be fed into vae     |
| `README.md`          | Overview of this folder.                                     |

---

##  Workflow Summary

1. **Load & Explore** raw data from each of the databases
2. **Clean & Transform** the data for modeling.
3. **Export** clean data to `../data/clean/` for downstream use.

##  Notes
- All notebooks are intended to be run in sequence.
- Output files and intermediate datasets are saved to `../data/raw` directory 
