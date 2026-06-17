# MLWA v12 revision checklist

Final editorial strengthening after v11.

## Completed changes

1. Contribution framing sharpened
   - Abstract, highlights, introduction, and contribution list now state that the paper contributes a matched estimand/protocol for compound tabular data-quality interaction.
   - The manuscript explicitly says it is not a new model, new robustness theory, or generic benchmark leaderboard.

2. Primary corruption process justified
   - The methods section now explains why noise-before-imbalance using observed corrupted labels is realistic.
   - Added pipeline examples: credit/claims coding, fraud/moderation/defect datasets, clinical registry case enrichment, and benchmark/internal dataset construction using observed labels.

3. Order/process dependence moved closer to main result
   - The main-results section now follows the chain: interaction definition -> main result -> process controls/order sensitivity -> mechanism -> secondary validations.
   - The order-sensitivity figure is now placed with the process-control result, not only in a later validation section.

4. Reproducibility clarified
   - Replaced vague wording such as "raw run-level result files where available".
   - Data/code availability now states that all run-level result files used for reported tables and figures are included, with specific row counts and experiment branches listed.

5. Missingness claims narrowed
   - The text now states that missingness is not the dominant interaction driver only under the tested MCAR, MAR-style, and MNAR-style mechanisms.
   - Removed any implication that missingness is generally secondary across all real-world pipelines.

6. Readability improved
   - Main section now opens with the core evidential chain.
   - Validation section renamed and framed as secondary support rather than separate headline contributions.

## Remaining author-side tasks before submission

- Replace anonymous author/affiliation information if the journal is not double-blind.
- Add a public repository or archival DOI URL after anonymous review if required by the journal.
- Confirm the journal's preferred Elsevier article class options and reference style.
