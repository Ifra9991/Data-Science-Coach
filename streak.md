# Data Science Learning Streak

## Current Status

- Current streak: 7 days
- Longest streak: 7 days
- Last completed date: 2026-05-23
- Learner level: Intermediate
- Weekly review 1: Due, covering Days 1-7 with 100 MCQs

## Completed Days

### Day 7 - 2026-05-23

**Topic:** GridSearchCV and hyperparameter tuning inside pipelines

**Completed:**

- Lesson
- Discussion
- Practical
- Test

**Test score:** 8/10

**Key learning:** GridSearchCV tests hyperparameter combinations using cross-validation, pipeline parameters use `step__parameter` syntax, and final test data should be used only after tuning.

**Weak areas to polish:** Exact API meanings for `grid.best_score_` and `grid.best_estimator_`, plus remembering to expand/refine the search when the best parameter is at the grid edge.

### Day 6 - 2026-05-22

**Topic:** Pipelines and ColumnTransformer

**Completed:**

- Lesson
- Discussion
- Practical
- Test

**Test score:** 7.5/8

**Key learning:** Pipeline ties preprocessing and modeling into one reproducible workflow; ColumnTransformer applies different preprocessing to numeric and categorical columns.

**Weak area to polish:** LogisticRegression fits during pipeline `fit`; prediction happens later with `predict()`.

### Day 5 - 2026-05-21

**Topic:** Regularization, L1, L2, C, and feature scaling

**Completed:**

- Lesson
- Discussion
- Practical
- Test

**Test score:** 8/8

**Key learning:** Smaller C means stronger regularization, larger C means weaker regularization, L1 can zero out coefficients, L2 shrinks weights, and scaling is important because penalties act on coefficient magnitude.

**Weak areas to polish:** None today.

### Day 4 - 2026-05-20

**Topic:** Bias-variance tradeoff and diagnosing underfitting vs overfitting

**Completed:**

- Lesson
- Discussion
- Practical
- Test

**Test score:** 7.5/8

**Key learning:** High bias means underfitting with low train and validation scores; high variance means overfitting with high train score and lower validation score.

**Weak area to polish:** Precise wording around regularization strength and model flexibility.

### Day 3 - 2026-05-19

**Topic:** Cross-validation, stratified folds, time-based validation, and final test sets

**Completed:**

- Lesson
- Discussion
- Practical
- Test

**Test score:** 6.5/8

**Key learning:** Cross-validation estimates model stability, StratifiedKFold preserves class ratios for imbalanced classification, and validation strategy should imitate deployment.

**Weak areas to polish:** The precise role of the final test set and explaining test-set overfitting as human/model-selection leakage rather than the model directly learning the test set.

### Day 2 - 2026-05-18

**Topic:** Precision, recall, F1-score, and classification thresholds

**Completed:**

- Lesson
- Discussion
- Practical
- Test

**Test score:** 6/8

**Key learning:** Precision measures the quality of positive predictions, recall measures coverage of actual positives, and metric choice depends on the cost of false positives versus false negatives.

**Weak areas to polish:** Threshold interpretation, F1-score business limitations, and precise wording around higher thresholds.

### Day 1 - 2026-05-17

**Topic:** Data leakage and feature windows

**Completed:**

- Lesson
- Discussion
- Practical
- Test

**Test score:** 6.5/7

**Key learning:** Leakage depends on whether information is available at prediction time, not only on the feature name.

**Weak area to polish:** Precise wording around prediction-time availability.
