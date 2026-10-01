# HealthConnect Clinic Experience Lab

## Improving Patient Appointment Attendance and Healthcare Support Using Data and AI

### Data Analytics Track — Week 8 Final Integration

**Analyst:** Chidinma Onyemachi
**Track:** Data Analytics
**Project:** HealthConnect Clinic Experience Lab
**Tools:** Power BI, DAX, Power Query, Excel
**Dataset:** HealthConnect Appointment Dataset
**Analysis Period:** January 1, 2025 – June 30, 2026
**Records:** 5,000 appointment records
**Unique Patients:** 1,696

---

## 1. Project Overview

HealthConnect Clinic is a fictional healthcare provider seeking to reduce missed appointments, improve patient appointment attendance, make better use of available appointment slots and provide more effective administrative support.

The HealthConnect project combines Data Analytics, Data Science, Machine Learning Engineering, Generative AI and Project Management into a multidisciplinary solution.

My contribution to the project is focused on Data Analytics and decision support.

The objective of my work was to analyze appointment attendance and no-show patterns, validate key analytical findings, develop decision-support visualizations and translate the results into business-relevant insights.

---

## 2. Business Problem

Missed appointments can affect appointment availability and the effective use of healthcare resources.

The analytics component therefore focuses on understanding:

* How many appointments were attended, cancelled or missed.
* The overall observed no-show rate.
* Appointment-type patterns.
* Reminder-status patterns.
* Previous no-show history.
* Segments with higher observed no-show rates.
* Analytical limitations that should be considered before using the findings for decision-making.

---

## 3. Dataset

The analysis uses the approved HealthConnect appointment dataset.

### Dataset Summary

| Metric                 |                      Value |
| ---------------------- | -------------------------: |
| Appointment records    |                      5,000 |
| Unique patients        |                      1,696 |
| Analysis period        | Jan 1, 2025 – Jun 30, 2026 |
| No-show appointments   |                      2,423 |
| Attended appointments  |                      2,314 |
| Cancelled appointments |                        263 |
| Observed no-show rate  |                     48.46% |

Patients can have multiple appointments, so appointment records should not be treated as completely independent observations.

The original HealthConnect project resources were retained separately and were not overwritten.

---

## 4. Data Analytics Process

The analytics workflow followed the HealthConnect project progression:

1. Data preparation
2. Exploratory analysis
3. KPI development
4. Power BI dashboard development
5. Segmentation analysis
6. Week 7 testing
7. Finding validation
8. Interpretation refinement
9. Final decision-support preparation
10. Week 8 integration

---

## 5. Tools Used

### Power BI

Used for:

* Dashboard development
* KPI visualization
* Interactive analysis
* Segmentation
* Business insights

### DAX

Used for:

* KPI measures
* No-show calculations
* Appointment outcome measures
* Dashboard metrics

### Power Query

Used for:

* Data preparation
* Transformation
* Data-quality checks

### Excel

Used where required for supporting data review and validation.

---

## 6. Final Dashboard

The final Power BI dashboard focuses on appointment attendance and no-show decision support.

### Main KPI Areas

* Total appointments
* Total cancellations
* No-show rate
* Reminder coverage
* Average booking lead days
* Appointment outcome totals

### Main Analytical Views

* Appointment outcome analysis
* Appointment type analysis
* Reminder status analysis
* Previous no-show history analysis
* Attendance/no-show patterns
* Segmentation-based decision support

The dashboard is intended to help users move beyond the overall no-show rate and identify meaningful patterns across appointment segments.

---

## 7. Week 7 Testing and Validation

Week 7 focused on testing and refining the analytical outputs developed during Week 6.

### Test 1 — KPI Validation

The major Power BI KPIs were tested against the underlying appointment data.

The tested measures included:

* Total appointments
* Total cancellations
* No-show rate
* Reminder coverage rate
* Average booking lead days
* Appointment outcome totals

### Result

The KPI results were validated and no correction was required.

---

## 8. Test 2 — Reminder Status × Appointment Type

Reminder status was tested against appointment type.

| Appointment Type        | Reminder Sent No-show | Reminder Not Sent No-show |
| ----------------------- | --------------------: | ------------------------: |
| Diagnostic              |                47.88% |                    55.56% |
| Specialist Consultation |                45.87% |                    51.63% |
| Follow-up               |                50.53% |                    53.13% |
| General Consultation    |                54.65% |                    49.16% |

### Finding

The relationship between reminder status and observed no-show rate was not consistent across all appointment types.

Diagnostic, Specialist Consultation and Follow-up showed lower observed no-show rates when a reminder was recorded as sent.

General Consultation showed the opposite observed pattern.

### Interpretation Refinement

The final analysis does not describe reminder status as having one uniform relationship with no-show behavior.

Instead, reminder status is treated as a contextual operational signal whose observed relationship varies by appointment type.

The analysis is observational and does not establish causation.

---

## 9. Test 3 — Appointment Type × Previous No-show History

Previous no-show history was tested across four appointment types.

### Diagnostic

* 0 previous no-shows: 44.67%
* 1 previous no-show: 54.64%
* 2 previous no-shows: 57.38%
* 3+ previous no-shows: 81.82%

### Specialist Consultation

* 0 previous no-shows: 43.89%
* 1 previous no-show: 49.81%
* 2 previous no-shows: 60.00%
* 3+ previous no-shows: 65.22%

### Follow-up

* 0 previous no-shows: 49.29%
* 1 previous no-show: 53.56%
* 2 previous no-shows: 65.19%
* 3+ previous no-shows: 70.00%

### General Consultation

* 0 previous no-shows: 40.43%
* 1 previous no-show: 54.60%
* 2 previous no-shows: 55.23%
* 3+ previous no-shows: 66.67%

### Finding

Across all four appointment types, higher previous no-show history corresponded with higher observed no-show rates.

This finding was validated and retained as an important segmentation signal.

---

## 10. Key Analytical Findings

### Finding 1 — Previous No-show History

Previous no-show history remained a consistent segmentation signal across appointment types.

Patients with greater previous no-show history generally showed higher observed no-show rates.

This supports using previous no-show history as an analytical segmentation variable.

### Finding 2 — Reminder Status

Reminder status did not demonstrate one uniform relationship with no-show behavior across all appointment types.

The relationship varied by appointment type.

Therefore, reminder-related findings should be interpreted within appointment context rather than as a universal effect.

---

## 11. Business Insights

The analysis provides several decision-support insights.

### 1. Segmentation matters

The overall no-show rate does not provide the full picture.

Breaking the data down by appointment type and previous no-show history reveals important differences.

### 2. Previous behavior provides a useful signal

Previous no-show history can help identify segments with higher observed no-show rates.

### 3. Operational interventions should be contextual

The reminder analysis shows that the observed relationship between reminder status and no-show behavior varies by appointment type.

Therefore, reminder-related decisions should be evaluated within the relevant appointment context.

### 4. Analytics should support, not replace, operational judgment

The findings provide evidence for decision-making but do not explain every reason a patient may miss an appointment.

---

## 12. Recommendations

Based on the validated analytical findings:

1. Use previous no-show history as one segmentation variable when identifying appointment groups requiring closer operational attention.

2. Review appointment-type-specific no-show patterns instead of relying only on the overall no-show rate.

3. Evaluate reminder-related performance by appointment type rather than assuming one uniform relationship.

4. Continue monitoring appointment attendance KPIs through the Power BI dashboard.

5. Combine analytics findings with other HealthConnect project components before making operational decisions.

6. Avoid interpreting observed relationships as causal effects.

---

## 13. Cross-Track Integration

### Primary Integration

**Data Analytics → Data Science**

The Data Analytics component provides validated findings that can support interpretation of the predictive component.

The key analytical outputs include:

* Previous no-show history as a validated segmentation signal.
* Appointment-type-specific reminder findings.
* Refined interpretation of reminder status.

### Integration Status

The Week 7 report identified the Data Analytics-to-Data Science validation as still pending.

Therefore, the final submission should only mark this integration as completed after:

1. The analytical output has been provided.
2. Data Science has used or evaluated the output.
3. The resulting change or impact has been documented.
4. Evidence of the exchange has been retained.

No cross-track activity is described as completed solely on the basis of a meeting or discussion.

---

## 14. Analytical Limitations

The following limitations should be considered:

* The dataset is synthetic.
* The analysis is observational.
* The results do not establish causation.
* There are 1,696 unique patients across 5,000 appointments.
* Patients may have multiple appointment records.
* 90 distance values are missing.
* 60 waiting-time values are missing.
* Reminder status does not confirm delivery, opening or reading.
* The dataset does not capture all potential reasons for nonattendance.
* Some higher-distance segments may contain smaller sample sizes.
* Appointment-type differences can affect the observed relationship between reminder status and no-show rate.

---

## 15. Week 7 → Week 8 Transition

### Main Week 7 Output

Validated and refined Power BI analytics and decision-support findings.

### Most Important Testing Result

Previous no-show history remained a consistent segmentation signal across appointment types.

### Major Issue Discovered

The relationship between reminder status and observed no-show rate was not uniform across appointment types.

### Refinement

The reminder finding was changed from a general interpretation to a contextual appointment-type interpretation.

### Component Ready

The core analytics findings and KPI validation are ready for final presentation and integration.

### Remaining Integration

Final documented exchange with the Data Science track must be completed before claiming the cross-track validation as finished.

---

## 16. Final Analytics Deliverable

The final Data Analytics package contains:

* Power BI dashboard
* Final KPIs
* Validated findings
* Key visualizations
* Business insights
* Recommendations
* Analytical limitations
* Cross-track integration documentation
* Executive summary
* Presentation materials
* Individual presentation video

---

## 17. Executive Summary

The HealthConnect Data Analytics work analyzed 5,000 appointment records covering January 2025 to June 2026.

The analysis found an observed no-show rate of 48.46%.

Week 7 testing validated the main Power BI KPIs.

Segmentation testing showed that previous no-show history was consistently associated with higher observed no-show rates across Diagnostic, Specialist Consultation, Follow-up and General Consultation appointments.

However, reminder status showed different patterns across appointment types. This resulted in a refinement of the Week 6 interpretation: reminder status should be treated as a contextual operational signal rather than a uniform relationship with no-show behavior.

The final analytics component provides HealthConnect with a data-driven view of appointment attendance and supports more targeted interpretation of no-show patterns.

The findings should be interpreted carefully because the dataset is synthetic and observational and does not establish causal relationships.

---

## 18. Portfolio Value

This project demonstrates practical experience in:

* Data cleaning
* Data validation
* Exploratory data analysis
* KPI development
* Power BI dashboard development
* DAX
* Power Query
* Segmentation analysis
* Analytical testing
* Data interpretation
* Business intelligence
* Decision support
* Evidence-based recommendations
* Cross-functional collaboration
* Professional documentation

---

## 19. Conclusion

The HealthConnect Data Analytics component progressed from dashboard development to analytical testing, validation and refinement.

The final analysis demonstrates that previous no-show history is a useful segmentation signal, while reminder-related patterns require appointment-type context.

The project also demonstrates the importance of validating analytical findings before translating them into business recommendations.

Future improvements could include additional real-world variables, stronger patient-level analysis, more complete attendance-related information and further validation of the cross-track predictive component.
