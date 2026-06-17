# V11 process-control output check

- Input raw file: `process_control_condition_metrics.csv`
- Raw rows repaired: 11,878
- Header columns original/full: 32 / 38
- Row-width distribution: {32: 4320, 38: 7558}
- Missing condition rows: 2

Missing condition rows:
| dataset_name   | model_name   |   seed | missing_condition                         |
|:---------------|:-------------|-------:|:------------------------------------------|
| vowel          | XGBoost      |      0 | compound_original_equal_size              |
| vowel          | XGBoost      |      3 | compound_clean_label_imbalance_then_noise |

## Macro-F1 process-control summary
| process_variant                        |   noise_drop |   imbalance_drop |   observed_compound_drop |   expected_additive_drop |   interaction |
|:---------------------------------------|-------------:|-----------------:|-------------------------:|-------------------------:|--------------:|
| clean_label_imbalance_then_noise       |       0.0706 |           0.1407 |                   0.2340 |                   0.2114 |        0.0226 |
| equal_training_size_control            |       0.0874 |           0.1048 |                   0.3581 |                   0.1922 |        0.1659 |
| fixed_current_index_matched_baseline   |       0.0706 |           0.1007 |                   0.3960 |                   0.1713 |        0.2247 |
| original_noise_then_observed_imbalance |       0.0706 |           0.1413 |                   0.3960 |                   0.2119 |        0.1840 |

## Dataset-equal Macro-F1 interaction CI
| process_variant                        |   dataset_equal_mean |   ci95_low |   ci95_high |   n_datasets |   positive_dataset_fraction |
|:---------------------------------------|---------------------:|-----------:|------------:|-------------:|----------------------------:|
| clean_label_imbalance_then_noise       |               0.0225 |     0.0073 |      0.0370 |           24 |                      0.8333 |
| equal_training_size_control            |               0.1657 |     0.1207 |      0.2126 |           24 |                      0.9583 |
| fixed_current_index_matched_baseline   |               0.2247 |     0.1668 |      0.2851 |           24 |                      0.9167 |
| original_noise_then_observed_imbalance |               0.1840 |     0.1363 |      0.2321 |           24 |                      0.9583 |

## Composition summary selected rows
| condition_name                                  | process_family         |   train_n |   clean_minority_retention_rate |   effective_clean_minority_ratio |   clean_true_majority_ratio_retained |   clean_true_min_class_count_retained |   mislabeled_retained_ratio |
|:------------------------------------------------|:-----------------------|----------:|--------------------------------:|---------------------------------:|-------------------------------------:|--------------------------------------:|----------------------------:|
| compound_clean_label_imbalance_then_noise       | clean_sampling_control | 2560.4087 |                          0.4734 |                           0.2214 |                               0.8130 |                              381.2938 |                      0.1993 |
| compound_fixed_current_indices_noisy_labels     | fixed_current_index    | 2341.8000 |                          0.3508 |                           0.1487 |                               0.7223 |                              376.1000 |                      0.1808 |
| compound_original_equal_size                    | equal_size             | 2339.1455 |                          0.3485 |                           0.1486 |                               0.7227 |                              376.1223 |                      0.1809 |
| compound_original_noise_then_observed_imbalance | original               | 2341.8000 |                          0.3508 |                           0.1487 |                               0.7223 |                              376.1000 |                      0.1808 |
| imbalance_only_clean_sampling                   | shared                 | 2558.1167 |                          0.4730 |                           0.2212 |                               0.8130 |                              380.9417 |                      0.0000 |