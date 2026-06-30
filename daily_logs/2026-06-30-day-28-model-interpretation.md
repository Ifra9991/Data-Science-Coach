# Day 28 - Model Interpretation and Explaining Predictions

**Date:** 2026-06-30

**Started:** 2026-06-29

**Status:** Completed

**Completed:**

- Lesson
- Discussion
- Practical
- Test

**Score:** 9.5/10

## Topic

Model interpretation, global vs local explanations, business-friendly prediction explanations, and avoiding causal language when explaining model outputs.

## Key Learning

Global explanations describe overall model behavior across many customers. Local explanations describe one specific prediction for one customer. Precision, recall, and F1 are not local metrics; they require many predictions. For a single customer, inspect predicted probability, threshold decision, final class, top local signals, and later whether the prediction became TP, FP, FN, or TN. A professional explanation should describe model reasoning without claiming causality.

## Strengths

- Correctly explained global vs local explanation.
- Correctly understood that precision, recall, and F1 cannot be calculated for one customer.
- Correctly identified local prediction information: predicted probability, threshold decision, contributing features, and SHAP/LIME-style values.
- Correctly avoided causal language in the test rewrite.
- Correctly distinguished between `the model flagged this customer` and `this customer will churn`.
- Practical explanations included probability, threshold, decision, signals, interpretation, action, and caution.

## Weak Areas To Polish

- In business explanations, include the threshold and causality caution consistently.
- Avoid emotional or psychological claims such as `shows his interest/uninterest`; use observed behavior such as `long time since last login` or `declining usage`.
- Use precise formatting for probabilities, such as `0.37` and `0.40`.
- For non-flagged customers, say `no strong warning signals` or `below threshold`, not vague phrases such as `good pattern`.

## Streak Note

Current streak is 1 day because Day 28 was completed on 2026-06-30 and no completed learning record exists for 2026-06-29. Longest streak remains 14 days.
