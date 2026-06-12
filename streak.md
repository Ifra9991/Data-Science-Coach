# Data Science Learning Streak

## Current Status

- Current streak: 2 days
- Longest streak: 14 days
- Last completed date: 2026-06-12
- Learner level: Intermediate
- Weekly review 1: Completed, 91/100
- Weekly review 2: Completed, 94/100

Note: Day 20 and Day 21 were both completed on 2026-06-12. The current streak remains 2 calendar days because streak counts completed dates, not number of lessons completed on the same date. The longest streak remains 14 days.

## Weekly Reviews

### Weekly Review 2 - 2026-06-05

**Scope:** Days 8-14

**Score:** 94/100

**Set scores:**

- Set 1: 18/20
- Set 2: 19/20
- Set 3: 19/20
- Set 4: 19/20
- Set 5: 19/20

**Strong areas:** Calibration, ROC-AUC, PR-AUC baseline interpretation, class imbalance strategies, threshold tuning, resampling safety, and error analysis.

**Weak areas to polish:** Class-1 precision vs recall wording, recall calculation, high precision/low recall interpretation, weighted average meaning in imbalanced classification, and careful cost-matrix arithmetic.

### Weekly Review 1 - 2026-05-24

**Scope:** Days 1-7

**Score:** 91/100

**Set scores:**

- Set 1: 19/20
- Set 2: 20/20
- Set 3: 20/20
- Set 4: 14/20
- Set 5: 18/20

**Strong areas:** Leakage, cross-validation, stratified folds, pipelines, regularization basics, and GridSearchCV workflow.

**Weak areas to polish:** Threshold direction under business constraints, false positive vs false negative interpretation in context, recall calculation/meaning, logistic regression C direction for high variance, and exact GridSearchCV scoring meaning.

## Completed Days

### Day 21 - 2026-06-12

**Topic:** Leakage-Safe Preprocessing Pipelines

**Completed:**

- Lesson
- Discussion
- Practical
- Test

**Test score:** 10/10

**Key learning:** ColumnTransformer applies different preprocessing to different column types, and a full pipeline keeps imputation, scaling, encoding, and modeling together so preprocessing is fitted only on training data.

**Weak areas to polish:** None today. Continue remembering that perfect metrics on a tiny test set are not reliable model evidence.

### Day 20 - 2026-06-12

**Topic:** Categorical Encoding for ML

**Started:** 2026-06-11

**Completed:**

- Lesson
- Discussion
- Practical
- Test

**Test score:** 8/10

**Key learning:** One-hot encoding is safer for unordered low/medium-cardinality categories, ordinal encoding is reasonable for truly ordered categories, high-cardinality features can explode dimensionality, and encoding inside a pipeline prevents train/test preprocessing leakage.

**Weak areas to polish:** Define one-hot encoding precisely as binary indicator columns. Remember that `handle_unknown="ignore"` prevents crashes but does not make the model understand unseen categories; it encodes them as none of the known categories.

### Day 19 - 2026-06-11

**Topic:** Outliers and Skewed Numeric Features

**Started:** 2026-06-09

**Completed:**

- Lesson
- Discussion
- Practical
- Test

**Test score:** 9/10

**Key learning:** Outlier treatment is a business and modeling decision. Mean vs median can reveal skew, business context helps separate real rare values from errors, log transforms reduce large-value dominance, and segment features can preserve useful high-value customer information.

**Weak areas to polish:** For real extreme values, prefer capping, log transform, or segment features over median imputation. Rare real segments also need caution because sample size can be too small to generalize.

### Day 18 - 2026-06-09

**Topic:** Missing Values In ML Features

**Started:** 2026-06-08

**Completed:**

- Lesson
- Discussion
- Practical
- Test

**Test score:** 9/10

**Key learning:** Missing values can be useful signals. Missing indicators, safe imputation, median for skewed numeric columns, `Unknown` for categorical missingness, and pipeline-based imputation all help prevent bad assumptions and leakage.

**Weak areas to polish:** Make zero-imputation rules more precise: missing after event aggregation often means no activity, while missing in a source field may mean unknown. Also say median is less affected by outliers.

### Day 17 - 2026-06-07

**Topic:** EDA for ML Features

**Completed:**

- Lesson
- Discussion
- Practical
- Test

**Test score:** 7.5/8

**Key learning:** EDA checks whether engineered features show sensible signal before modeling. Comparing target-group summaries, mean vs median, segment churn rates, and sample sizes helps catch misleading patterns early.

**Weak areas to polish:** Interpret segment churn rates as group-level results, not single-customer statements; keep sample-size caution attached to strong-looking patterns.

### Day 16 - 2026-06-07

**Topic:** Feature Engineering for ML Models

**Started:** 2026-06-06

**Completed:**

- Lesson
- Discussion
- Practical
- Test

**Test score:** 9.5/10

**Key learning:** Good features convert business signals into time-safe numerical inputs. Recency, frequency, trend/change, ratio, and segment features all help the model see customer behavior more clearly.

**Weak areas to polish:** Event-level to customer-level aggregation wording and remembering that negative usage drop means recent usage increased.

### Day 15 - 2026-06-05

**Topic:** Weekly Review 2: Days 8-14 cumulative MCQ assessment

**Completed:**

- Review
- 100-MCQ test

**Test score:** 94/100

**Key learning:** The second-week concepts are much stronger now, especially calibration, ROC-AUC, PR-AUC, imbalance handling, and error analysis.

**Weak areas to polish:** Precision/recall wording, recall calculation, high precision/low recall interpretation, weighted average meaning, and cost-matrix arithmetic.

### Day 14 - 2026-06-02

**Topic:** Error analysis for false positives and false negatives

**Started:** 2026-05-31

**Completed:**

- Lesson
- Discussion
- Practical
- Test

**Test score:** 8/10

**Key learning:** Metrics tell how much the model is wrong; error analysis tells where and why it is wrong.

**Weak areas to polish:** Churn-specific FP/FN wording and turning error patterns into precise next checks such as support topic, ticket resolution, and segment-specific threshold analysis.

### Day 13 - 2026-05-31

**Topic:** Handling Imbalanced Classification

**Started:** 2026-05-29

**Completed:**

- Lesson
- Discussion
- Practical
- Test

**Test score:** 8/10

**Key learning:** Accuracy can be misleading in imbalanced classification; class weights can improve minority-class recall but often increase false positives; threshold tuning changes the cutoff without retraining.

**Weak areas to polish:** Resampling safety, precise class-1 precision/recall wording, and understanding why threshold tuning should still be tested on a model with better PR-AUC.

### Day 12 - 2026-05-29

**Topic:** PR-AUC and rare positive-class evaluation

**Started:** 2026-05-28

**Completed:**

- Lesson
- Discussion
- Practical
- Test

**Test score:** 8/10

**Key learning:** PR-AUC focuses on positive-class performance and is often more informative for rare events because it summarizes the precision-recall tradeoff across thresholds.

**Weak areas to polish:** Explaining PR-AUC relative to the positive-rate baseline and interpreting why a practical PR-AUC is better than baseline.

### Day 11 - 2026-05-28

**Topic:** ROC-AUC and ranking quality

**Started:** 2026-05-27

**Completed:**

- Lesson
- Discussion
- Practical
- Test

**Test score:** 8/10

**Key learning:** ROC-AUC measures ranking quality: the chance that a randomly chosen positive case scores above a randomly chosen negative case.

**Weak areas to polish:** ROC-AUC of 0.5 means random ranking, TPR/FPR formulas, and what to inspect beyond ROC-AUC for rare fraud detection.

### Day 10 - 2026-05-26

**Topic:** Probability calibration

**Completed:**

- Lesson
- Discussion
- Practical
- Test

**Test score:** 10/10

**Key learning:** Calibration means predicted probabilities match real-world frequencies; ranking asks who is riskier, while calibration asks how risky they really are.

**Weak areas to polish:** None today.

### Day 9 - 2026-05-25

**Topic:** Business cost matrix and threshold decisions

**Completed:**

- Lesson
- Discussion
- Practical
- Test

**Test score:** 6/10

**Key learning:** Threshold choice should be based on business cost, not F1 alone or a vague sense of balance.

**Weak areas to polish:** Threshold direction when false negatives or false positives are expensive, cost calculation accuracy, and explaining why the lowest/highest threshold is not automatically best.

### Day 8 - 2026-05-24

**Topic:** Weekly Review 1: Days 1-7 cumulative MCQ assessment

**Completed:**

- Review
- 100-MCQ test

**Test score:** 91/100

**Key learning:** Scenario-based questions reveal metric reasoning better than definition-only questions. Future tests should stay analytical and avoid answer-pattern clustering.

**Weak areas to polish:** Threshold strategy, false positive/false negative context, and recall interpretation.

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
