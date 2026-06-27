# Day 26 - Threshold Tuning After Model Selection

**Date:** 2026-06-27

**Status:** Completed

**Completed:**

- Lesson
- Discussion
- Practical
- Test

**Score:** 10/10

## Topic

Threshold tuning after model selection, using predicted probabilities, precision/recall movement, false positive and false negative costs, and validation-safe threshold selection.

## Key Learning

Threshold is applied to predicted probability, not directly to precision or recall. Lowering the threshold usually increases recall and false positives while reducing false negatives. Raising the threshold usually increases precision, reduces false positives, and increases false negatives. The best threshold depends on business cost, not only F1. Threshold tuning must be done on validation data because threshold choice is part of model development; the final test set should remain untouched until the model and threshold are frozen.

## Strengths

- Correctly identified that threshold is applied to predicted probability.
- Correctly converted probabilities into churn/not-churn decisions at different thresholds.
- Correctly calculated threshold business cost from FP and FN costs.
- Correctly understood that cost-best threshold can differ from F1-best threshold.
- Correctly explained why threshold tuning on the final test set causes model-selection leakage.
- Improved precision around the phrase: probability belongs to one customer; precision and recall belong to model performance over a dataset.

## Weak Areas To Polish

- Keep using the precise phrase `model-selection leakage` when threshold choices are influenced by final-test performance.
- Remember the mature rule: lowering threshold usually increases recall, but precision can move unexpectedly depending on whether newly included cases are true positives or false positives.

## Streak Note

Current streak is 1 day because the previous completed daily log was 2026-06-21 and no completed learning records exist for 2026-06-22 through 2026-06-26. Longest streak remains 14 days.
