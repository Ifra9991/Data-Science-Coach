# Day 25 - Cross-Validated Model Comparison

**Date:** 2026-06-21

**Status:** Completed

**Completed:**

- Lesson
- Discussion
- Practical
- Test

**Score:** 9/10

## Topic

Cross-validated model comparison using StratifiedKFold, cross_validate, mean score, standard deviation, and multiple metrics.

## Key Learning

Cross-validation protects against trusting one lucky or unlucky validation split. Mean CV score shows average performance, while standard deviation shows stability across folds. StratifiedKFold is safer for imbalanced churn classification because it preserves class ratios across folds. Passing the full preprocessing and model pipeline into cross_validate keeps imputation, scaling, encoding, and fitting leakage-safe inside each fold.

## Strengths

- Correctly explained that one validation split can be lucky or unlucky.
- Understood that CV standard deviation measures fold-to-fold variation.
- Correctly connected high standard deviation with instability.
- Correctly explained why StratifiedKFold is useful for imbalanced churn data.
- Correctly prioritized recall when missing churners is expensive.
- Correctly prioritized precision when retention offers are expensive and team capacity is small.
- Gave a strong leakage-safe explanation for using a full pipeline inside cross_validate.

## Weak Areas To Polish

- Be more precise that normal KFold can create folds with too few or even zero churners when churn rate is very low.
- When explaining multiple metrics, explicitly say that F1 can hide the precision-recall tradeoff.
- Avoid saying validation split misleads the final test result; better wording is that it can mislead model selection or validation estimates.

## Streak Note

Current streak is 1 day because the previous recorded completion was 2026-06-17 and no completed learning records exist for 2026-06-18, 2026-06-19, or 2026-06-20. Longest streak remains 14 days.
