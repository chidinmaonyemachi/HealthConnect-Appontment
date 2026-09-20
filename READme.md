# HealthConnect Clinic Experience Lab — Week 7

## Advanced Analytics & Decision Support — Data Analytics Track

### Project Overview

This project analyses appointment attendance behaviour for HealthConnect Clinic using 5,000 appointment records covering **1 January 2025 to 30 June 2026**.

Week 6 focused on advanced segmentation, KPI development and Power BI decision support. Week 7 builds forward from that work by **testing, validating and refining the Week 6 analytical outputs** rather than repeating the original analysis.

---

## Week 7 Objective

The Week 7 objective is to:

- Validate the Week 6 Power BI KPIs.
- Test whether important Week 6 findings remain consistent when examined across appointment types.
- Identify analytical patterns that are not uniform across segments.
- Refine the interpretation of findings where necessary.
- Retest validated findings.
- Document testing evidence and prepare the analysis for Week 8 integration.

---

## Week 6 → Week 7 Progression

**Week 6 Output → Test → Identify Finding → Refine → Retest → Validate → Document → Prepare for Week 8**

Week 7 therefore does not rebuild the dashboard or repeat the original exploratory analysis.

---

## Dataset

| Item | Value |
|---|---:|
| Records | 5,000 |
| Unique appointment IDs | 5,000 |
| Unique patients | 1,696 |
| Appointment period | 2025-01-01 to 2026-06-30 |
| No-Show appointments | 2,423 |
| Attended appointments | 2,314 |
| Cancelled appointments | 263 |

Patients can have multiple appointments, so appointment records are not fully independent observations.

---

## Week 7 Testing Completed

### Test 1 — KPI Validation

The main Power BI KPIs were tested for correct operation.

Validated KPI areas:

- Total appointments
- Total cancellations
- No-show rate
- Reminder coverage rate
- Average booking lead days
- Appointment outcome totals

**Result:** All tested KPIs were working correctly.

**Action:** No correction required.

**Status:** Validated.

---

### Test 2 — Reminder Status × Appointment Type

The purpose of this test was to determine whether the Week 6 reminder-status pattern remained consistent across appointment types.

#### Diagnostic Test

- Total appointments: **593**
- Reminder sent: **449** — no-show **47.88%**
- Reminder not sent: **144** — no-show **55.56%**

#### Specialist Consultation

- Total appointments: **900**
- Reminder sent: **654** — no-show **45.87%**
- Reminder not sent: **246** — no-show **51.63%**

#### Follow-up

- Total appointments: **1,421**
- Reminder sent: **1,037** — no-show **50.53%**
- Reminder not sent: **384** — no-show **53.13%**

#### General Consultation

- Total appointments: **2,086**
- Reminder sent: **1,494** — no-show **54.65%**
- Reminder not sent: **592** — no-show **49.16%**

### Finding

The reminder relationship was **not consistent across appointment types**.

For Diagnostic Test, Specialist Consultation and Follow-up, the reminder-sent group had a lower observed no-show rate. For General Consultation, the reminder-sent group had a higher observed no-show rate.

### Refinement

The Week 6 narrative should not describe reminder status as having one uniform relationship with no-shows across all appointment types.

The finding remains **associational, not causal**. Reminder status does not confirm delivery, patient engagement or whether the reminder was read.

**Status:** Tested — refinement required.

---

### Test 3 — Appointment Type × Previous No-Show History

The purpose of this test was to determine whether the Week 6 previous no-show finding remained consistent across appointment types.

#### Diagnostic Test

- Total appointments: **593**
- Previous no-show 0: **44.67%**
- Previous no-show 1: **54.64%**
- Previous no-show 2: **57.38%**
- Previous no-show 3+: **81.82%**

#### Specialist Consultation

- Total appointments: **900**
- Previous no-show 0: **43.89%**
- Previous no-show 1: **49.81%**
- Previous no-show 2: **60.00%**
- Previous no-show 3+: **65.22%**

#### Follow-up

- Total appointments: **1,421**
- Previous no-show 0: **49.29%**
- Previous no-show 1: **53.56%**
- Previous no-show 2: **65.19%**
- Previous no-show 3+: **70.00%**

#### General Consultation

- Total appointments: **2,086**
- Previous no-show 0: **40.43%**
- Previous no-show 1: **54.60%**
- Previous no-show 2: **55.23%**
- Previous no-show 3+: **66.67%**

### Finding

The same directional pattern was observed across all four appointment types: higher previous no-show history corresponded with higher observed no-show rates.

### Refinement

No analytical correction was required.

The Week 6 finding on previous no-show history was retained and **validated through segmentation testing**.

**Status:** Validated.

---

## Testing & Validation Matrix

| ID | Component Tested | Testing Objective | Expected Result | Actual Result | Status | Issue / Finding | Action |
|---|---|---|---|---|---|---|---|
| T01 | Power BI KPIs | Confirm KPI calculations and operation | KPIs should display correctly | KPIs worked correctly | Pass | No issue identified | No change |
| T02 | Reminder status × appointment type | Test whether reminder pattern is consistent across appointment types | Similar directional pattern across types | Pattern differed for General Consultation | Finding | Reminder relationship is not uniform | Refined interpretation |
| T03 | Appointment type × previous no-show history | Test stability of previous no-show finding | Higher previous no-show history should remain associated with higher no-show rates | Pattern observed across all four types | Pass | No issue identified | Retain finding |

---

## Week 7 Findings

### Finding 1 — Previous no-show history remains a stable segmentation signal

The relationship between previous no-show history and current no-show rate remained visible across Diagnostic Test, Specialist Consultation, Follow-up and General Consultation.

This strengthens the Week 6 interpretation that previous no-show history is a useful analytical segmentation variable.

### Finding 2 — Reminder status does not show one uniform pattern across appointment types

The overall Week 6 reminder association does not remain identical within every appointment type.

This means reminder status should be interpreted with appointment context rather than as a universal relationship.

---

## Refinement Made in Week 7

The main analytical refinement is to make the reminder finding more precise.

### Before

Reminder status was described at the overall dataset level as an observed association with no-show behaviour.

### After Week 7 Testing

The analysis now recognises that the observed reminder relationship varies by appointment type. Therefore, reminder status should be treated as a contextual operational signal rather than a uniform pattern across all appointment categories.

No change was required for the previous no-show finding because the pattern remained consistent across appointment types.

---

## Cross-Track Validation

The Week 7 guide requires at least one meaningful cross-track testing or validation activity.

### Planned connection

**Data Analytics → Data Science**

### Dependency

The Data Analytics findings may influence the variables, features or analytical assumptions used by the Data Science track.

### Current status

The analytical tests above have been completed within the Data Analytics work. The cross-track validation activity still needs to be documented after the Data Science testing/validation interaction is completed.

**Important:** A meeting or discussion alone will not be recorded as cross-track validation. The final evidence should show the component tested, finding, action, retest result and what changed.

---

## Limitations

The Week 6 limitations remain relevant:

- The dataset is synthetic.
- The analysis is observational and does not establish causation.
- 1,696 patients account for 5,000 appointments, so records are not fully independent.
- 90 records have missing distance values.
- 60 records have missing waiting-time values.
- Reminder sent does not confirm delivery or whether the patient read the reminder.
- Transport, illness and other reasons for non-attendance are not available.
- Higher-distance segments have smaller sample sizes.

Week 7 adds an analytical limitation: the reminder relationship varies across appointment types, so overall reminder comparisons should not be interpreted without considering segmentation.

---

## Week 8 Preparation

Before Week 8, the Data Analytics track should:

1. Complete the required cross-track validation with Data Science.
2. Record the testing evidence and any output received/provided.
3. Retest any refined cross-track component where applicable.
4. Update the final Power BI narrative to reflect the Week 7 reminder finding.
5. Keep previous no-show history as a validated analytical signal.
6. Maintain the documented limitations and avoid causal claims.
7. Commit the updated report, README and supporting evidence to GitHub.

---

## Conclusion

Week 7 moved the Data Analytics work from Week 6 analysis into testing and validation.

The Power BI KPIs were validated. Previous no-show history remained consistent across appointment types and was therefore validated as a stable observed pattern. Reminder status required refinement because its observed relationship with no-show behaviour was not consistent across all appointment types.

The main Week 7 improvement is therefore **more precise interpretation**, rather than rebuilding the dashboard or repeating the Week 6 analysis.

