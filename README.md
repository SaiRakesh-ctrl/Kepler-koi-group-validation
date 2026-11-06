# Group-Aware Validation of Kepler KOI Data

High school ISEF project examining the effect of host-star grouping on classification performance in the Kepler KOI catalog (1–4 R⊕, Teff 4700–6500 K).

## Main Result

Host-star-grouped cross-validation produces almost no change in performance on the filtered KOI sample (ΔROC-AUC ≈ 0.002–0.003). The same method shows a much larger gap on a subject-grouped Parkinson’s voice dataset, indicating that the importance of group-aware splits depends on the data structure.

## Important Caveat

The catalog fraction reported here is a descriptive statistic conditional on stars that already appear in the filtered KOI table. It is **not** a true occurrence rate among all Kepler target stars (no completeness or transit-probability corrections applied).

## Notebooks

| Notebook | Description |
|----------|-------------|
| `01_data_preparation.ipynb` | Sample definition and filtering (1–4 R⊕, Teff 4700–6500 K) |
| `02_baseline_catalog_fraction.ipynb` | Descriptive confirmed-host catalog fraction |
| `03_group_aware_validation.ipynb` | Main group-aware vs random cross-validation comparison |
| `04_before_after_comparison.ipynb` | Summary of validation metrics and plots |
| `05_robustness_thresholds.ipynb` | Threshold and metric robustness checks |
| `06_parkinsons_comparison.ipynb` | Cross-domain contrast with Parkinson’s voice dataset |
| `07_literature_audit.ipynb` | Literature comparability checklist |
| `08_catalog_recovery.ipynb` | Recovery of confirmed planets under group-aware scoring |
| `09_k_dwarf_example.ipynb` | Narrow K-dwarf subpopulation example |
| `10_repeated_group_validation.ipynb` | Multi-seed stability of group-aware results |
| `11_feature_ablation.ipynb` | Feature-family ablation tests |
| `12_probability_calibration.ipynb` | Probability calibration diagnostics |
| `13_k_dwarf_subpopulations.ipynb` | Further K-dwarf subgroup analysis |
| `14_integrated_statistical_comparison.ipynb` | Integrated metrics with host-cluster bootstrap |
| `15_k_dwarf_occurrence_rate.ipynb` | K-dwarf catalog summary and caveats |
| `16_tce_candidate_investigation.ipynb` | TCE / candidate screening notes |

All notebooks are designed to run top-to-bottom on Kaggle or a standard Python environment with pandas, scikit-learn, and matplotlib.

## License

This project is released under the MIT License.
