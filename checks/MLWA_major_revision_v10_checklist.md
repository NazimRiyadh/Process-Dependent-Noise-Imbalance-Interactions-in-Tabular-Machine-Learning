# MLWA / Q1 Major Revision Checklist - v10

## Reviewer concern addressed

1. Sharper novelty positioning
   - Title shortened.
   - Abstract and introduction now emphasize process-dependent tabular data-quality interaction protocol rather than claiming generic novelty of interaction statistics.

2. Reproducibility gap
   - Added v10 reproducibility package.
   - Included PMLB manifest, v10 selection audit, raw/processed outputs, OpenML outputs, tuned outputs, and v10 notebook.
   - Removed placeholder repository language from manuscript.

3. Dataset-selection transparency
   - Added dataset-selection audit table.
   - Rebuilt PMLB manifest from v10 audit.
   - Main text now explains retained-suite logic and external OpenML replication.

4. Additive-null statistical support
   - Added cluster-robust run-level regression with dataset-clustered standard errors.
   - Added transformed-scale logit Macro-F1 check.
   - Added row-equal, dataset-equal, and dataset-model-equal weighting check.

5. Mechanism evidence
   - Added PMLB-side mechanism diagnostics.
   - Added binary/multiclass mechanism split.
   - Added dataset-level mechanism-interaction correlations.
   - Added mechanism correlation/scatter and severity curve figure.

6. Imbalance construction clarity
   - Added exact induced-imbalance algorithm table.
   - Explicitly states majority recomputation after noise, multiclass non-majority sampling, infeasible-target handling, and zero-division convention.

7. Practical implications / mitigation
   - Added mitigation mini-study over 24 PMLB datasets, 4 models, 5 seeds, 3 mitigation strategies.
   - Main result: class weighting and random oversampling reduce but do not eliminate the noise+imbalance interaction.

8. Final polish
   - Shorter abstract.
   - Removed placeholder repository URL language.
   - Compiled PDF and visually checked rendered pages.

## Remaining author-side item
- Replace anonymous author block with real author names/affiliations if the target journal does not use anonymized review.
- Upload reproducibility package to a public/anonymized repository if required by the journal system.
