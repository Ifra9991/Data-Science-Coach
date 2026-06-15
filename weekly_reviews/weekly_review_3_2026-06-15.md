# Weekly Review 3 - 2026-06-15

**Scope:** Days 16-22  
**Status:** Completed  
**Score:** 98/100  
**Current streak after completion:** 2 days  
**Longest streak:** 14 days

## Set Scores

- Set 1: 20/20
- Set 2: 19/20
- Set 3: 20/20
- Set 4: 19/20
- Set 5: 20/20

## Missed Questions

### Q36 - Rolling Time Validation

Correct idea: rolling time validation trains on earlier time periods and validates on later time periods. It is used when the real deployment situation depends on time order.

### Q67 - Event Aggregation Missingness

Correct idea: after aggregating event rows and left-merging back to customers, missing event counts usually mean the customer had zero observed events in that window. This is different from a source field being unknown.

## Strong Areas

- Feature engineering: recency, frequency, trend, ratio, and segment features
- EDA for ML features
- Missing-value indicators and safe imputation
- Outlier diagnosis, skew, log transforms, and high-value flags
- One-hot, ordinal, and high-cardinality encoding decisions
- ColumnTransformer and leakage-safe preprocessing pipelines
- Train, validation, and final test set roles
- Model-selection leakage and time-aware validation

## Weak Areas To Polish

- Rolling time validation wording
- Distinguishing event-aggregation missingness from source-field missingness

## Teacher Note

This was a strong weekly review. A 98/100 on these topics means the foundation is becoming real, not just memorized. The remaining mistakes are narrow engineering details, so the next lessons can continue moving forward while briefly revisiting those two points.
