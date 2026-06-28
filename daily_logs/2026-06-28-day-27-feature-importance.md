# Day 27 - Feature Importance vs Permutation Importance

**Date:** 2026-06-28

**Status:** Completed

**Completed:**

- Lesson
- Discussion
- Practical
- Test

**Score:** 9.5/10

## Topic

Feature importance, permutation importance, leakage detection through suspicious top features, correlated-feature caveats, and feature triage for wide datasets.

## Key Learning

Feature importance tells us which features the model relies on for prediction, but it does not prove causality. Built-in Random Forest importance is model-internal and based on tree split behavior. Permutation importance is performance-based and measures how much validation score drops when a feature is shuffled. High importance for post-outcome fields such as cancellation reason or refund after cancellation is a leakage warning, not a success signal.

## Strengths

- Correctly separated feature importance from causality.
- Correctly identified `cancellation_reason_encoded` and `refund_after_cancellation` as leakage risks.
- Correctly explained that leakage features should be removed, not merely shuffled.
- Correctly explained that built-in feature importance looks inside the model while permutation importance measures validation-performance damage.
- Correctly understood that correlated features can look individually weak because a similar feature still carries the same signal.
- Correctly connected a large F1 drop after shuffling to high predictive importance.

## Weak Areas To Polish

- When handling many columns, include the full triage workflow: leakage check, business logic, data-quality checks, EDA signal, model importance, and validation-performance checks.
- When a low-importance feature appears, do not drop it automatically; first check business meaning, correlation, permutation importance, and validation impact.
- For leakage features, the fix is to remove them, retrain, and re-evaluate. Shuffling is only a diagnostic tool.

## Streak Note

Current streak is 2 days because Day 26 was completed on 2026-06-27 and Day 27 was completed on 2026-06-28. Longest streak remains 14 days.
