# Group-Aware Validation of Kepler KOI Data

High school ISEF project examining the effect of host-star grouping on classification performance in the Kepler KOI catalog (1–4 R⊕, Teff 4700–6500 K).

## Main Result
Host-star-grouped cross-validation produces almost no change in performance on the filtered KOI sample (ΔROC-AUC ≈ 0.002–0.003). The same method shows a much larger gap on a subject-grouped Parkinson’s voice dataset, indicating that the importance of group-aware splits depends on the data structure.

## Important Caveat
The catalog fraction reported here is a descriptive statistic conditional on stars that already appear in the filtered KOI table. It is **not** a true occurrence rate among all Kepler target stars (no completeness or transit-probability corrections applied).

## Notebooks
- `01_data_preparation.ipynb` – sample definition
- `02_baseline_catalog_fraction.ipynb`
- `03_group_aware_validation.ipynb`
- `04_comparison.ipynb`
- `05_robustness.ipynb`
- `06_parkinsons_comparison.ipynb`
- `07_literature_audit.ipynb`

All notebooks are designed to run top-to-bottom on Kaggle or a standard Python environment with pandas, scikit-learn, and matplotlib.
