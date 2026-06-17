# V13 final submission polish checklist

## Completed manuscript changes

- Updated title to foreground the strongest contribution: process-dependent noise-imbalance interaction.
- Shortened and sharpened the abstract around the core chain: estimand/protocol, main PMLB result, process controls, mechanism, OpenML replication, mitigation, and narrow missingness interpretation.
- Clarified that the contribution is an estimand/protocol and controlled diagnostic benchmark, not a new classifier, loss function, optimizer, or general robustness theory.
- Strengthened the realistic-pipeline justification for observed-label imbalance after label noise.
- Kept order sensitivity and process-control experiments as part of the main empirical result, not a late validation.
- Narrowed missingness claims: missingness is included in the factorial benchmark, but under the tested MCAR, MAR-style, and MNAR-style mechanisms it is not the dominant excess-interaction driver.
- Reduced main-text density by moving selected detailed tables to the reproducibility package: extended manifests, exclusions, sampling diagnostics, normalized-score details, statistical stress-check details, binary/multiclass mechanism split, OpenML mechanism table, OpenML metric table, MAR/MNAR detailed tables, tuning detailed table, validation table, model-ranking details, and dataset-heterogeneity details.
- Preserved main-text focus on: interaction definition -> main result -> order/process controls -> mechanism -> OpenML replication -> mitigation/practical implications.
- Rewrote the reproducibility and data/code availability text to avoid incomplete wording such as "where available" or "upon request".

## Reproducibility package improvements

- Created a self-contained v13 reproducibility archive.
- Included final PDF, main TeX file, and full LaTeX source ZIP.
- Included notebooks/scripts for OpenML replication, V10 mechanism/statistics/mitigation analysis, V11 process controls, tuning sensitivity, and MAR sensitivity.
- Included main run-level result CSVs and processed interaction summaries.
- Included OpenML replication raw and processed outputs.
- Included process-control repaired raw metrics and interaction summaries.
- Included mechanism diagnostics, mitigation outputs, tuning outputs, and missingness outputs where used in the paper.
- Included dataset manifests and screening records.
- Included figure sources.
- Added README, package summary, requirements, runtime notes, FILE_MANIFEST.csv, and SHA256SUMS.txt.

## Remaining author-side tasks before actual journal submission

1. Replace anonymous author block if the journal is not double-blind.
2. Upload the v13 reproducibility package to the journal system as supplementary material.
3. If non-anonymous or after acceptance, deposit the reproducibility archive in Zenodo/OSF/Figshare/institutional repository and insert the DOI/URL.
4. Check Elsevier/MLWA submission limits for supplementary file size and split the package if needed.
5. Confirm all figures meet journal resolution requirements.
