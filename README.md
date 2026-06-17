# Q1 Defense Reproducibility Package

This archive accompanies the manuscript:

**Process-Dependent Noise-Imbalance Interactions in Tabular Machine Learning: A Compound Data-Quality Benchmark**

## What is fully included

This package includes all run-level result files and processed analysis files used to generate the reported tables and figures in the final manuscript. In particular, it includes:

1. Main PMLB benchmark outputs: completed 69,120-row nine-model benchmark and derived interaction summaries.
2. External OpenML replication outputs: completed 57,600-row replication and derived interaction summaries.
3. Final process-control outputs: repaired raw condition metrics, interaction summaries, weighting summaries, bootstrap summaries, and composition diagnostics.
4. PMLB mechanism/statistical/mitigation outputs: PMLB mechanism diagnostics, cluster-robust and mixed-model outputs, logit-scale checks, mitigation raw results and summaries.
5. Missingness sensitivity outputs: imputation-ablation, MAR/MNAR-style sensitivity outputs available from the executed notebooks/packages.
6. Clean-data tuning sensitivity outputs: raw tuned-sensitivity results, selected hyperparameters, and processed drops/interactions.
7. Dataset manifests and screening records for PMLB and OpenML.
8. Figure source files used by the manuscript.
9. Executable Kaggle notebooks/scripts used to reproduce the main validation branches.
10. Environment files listing key Python packages.

## What is not redistributed

The public PMLB and OpenML datasets themselves are not redistributed. They are referenced by dataset manifest and loader instructions. The notebooks fetch them from their public sources.

## Folder guide

- `manuscript/`: final PDF, main TeX file, and full LaTeX source ZIP.
- `code/`: notebooks/scripts used for OpenML replication, V10 statistical/mechanism/mitigation checks, V11 process controls, tuned sensitivity, and MAR sensitivity.
- `data_manifest/`: dataset manifests and selection/screening files.
- `raw_results/`: run-level CSV files used as inputs to the reported analyses.
- `processed_results/`: interaction tables, summary tables, model outputs, mechanism diagnostics, mitigation summaries, and validation summaries.
- `figures/`: manuscript figure files.
- `environment/`: package requirements and runtime notes.
- `checks/`: revision/checklist notes.

## Main reproducibility statement

All run-level result files used to compute the reported tables and figures are included in this archive. Public datasets are referenced through PMLB/OpenML manifests rather than redistributed. The `SHA256SUMS.txt` file lists hashes for all files in the archive.

## Public repository

A public copy of the reproducibility package is available at:

https://github.com/NazimRiyadh/Process-Dependent-Noise-Imbalance-Interactions-in-Tabular-Machine-Learning

For archival stability, the authors may additionally create a DOI-bearing release through Zenodo, Figshare, OSF, or an institutional repository.
