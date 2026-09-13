# HealthConnect Clinic Experience Lab

## Advanced Analytics & Decision Support — Week 6

### Project objective

Week 6 builds on the Week 5 exploratory analysis, KPI development and initial dashboard. The focus is on deeper investigation of the strongest findings, KPI validation, analytical decision support, dashboard improvement and cross-track collaboration with the Data Science track.

### Week 5 → Week 6 transition

Week 5 established the initial analytical baseline for HealthConnect, including data preparation, KPI development, exploratory analysis, dashboard development and business recommendations.

The strongest initial findings were related to previous no-show history, booking lead time, reminder status, distance to clinic and appointment type.

Week 6 focuses on investigating these findings more deeply, validating their relevance, examining additional patient and appointment segments, improving the analytical dashboard and providing relevant analytical evidence to the Data Science track.

### Week 6 analytical focus

The main areas investigated are:

- Previous no-show history
- Booking lead time
- Reminder status
- Distance to clinic
- Appointment type
- Age group

### Advanced analysis

#### 1. Previous no-show history

Week 5 showed a substantial difference in observed no-show rates between appointments with no previous no-shows and appointments with three or more previous no-shows.

Week 6 investigates this relationship further by examining previous no-show groups and their relationship with other appointment characteristics.

#### 2. Booking lead time

Week 5 identified an increase in observed no-show rates across longer booking lead-time bands.

Week 6 investigates whether this pattern remains when considered alongside other relevant appointment characteristics, particularly previous no-show history.

#### 3. Reminder status

Week 5 showed a lower observed no-show rate among appointments where reminders were sent.

Week 6 investigates whether this difference remains consistent across relevant patient and appointment segments.

The relationship is treated as an association and not as evidence of causation.

#### 4. Distance to clinic

Week 5 identified higher observed no-show rates among longer-distance groups.

Week 6 reviews this finding further, particularly considering the relatively small number of appointments in the 30+ km group.

#### 5. Appointment type

Follow-up appointments had the highest observed no-show rate in Week 5.

Week 6 investigates whether this difference remains when considered alongside other relevant appointment characteristics.

#### 6. Age group

Week 6 extends the segmentation analysis by examining no-show rates across age groups.

This analysis is used to determine whether meaningful differences in appointment attendance behaviour exist across patient age segments and whether age group provides additional context for the patterns identified in Week 5.

### KPI validation

The Week 5 KPIs were reviewed and validated for:

- Total appointments
- Total cancellations
- No-show rate
- Reminder coverage rate
- Average booking lead days

The calculation logic and relevant denominators were reviewed to ensure consistency in the Week 6 analysis.

### Dashboard improvements

The Week 6 dashboard was enhanced to support deeper analytical investigation and decision-making.

New and refined analytical views include:

- No-show rate by previous no-show group
- No-show rate by booking lead-time band
- No-show rate by age group
- No-show rate by appointment type
- No-show rate by reminder status
- No-show rate by distance to clinic
- No-show rate by waiting-time band
- Comparison of attended, no-show and cancelled appointments
- Reminder sent versus not sent analysis

The dashboard moves beyond the initial Week 5 reporting view by providing additional segmentation and deeper analysis of factors associated with appointment no-show behaviour.

### Key analytical focus

The Week 6 analysis places particular attention on:

- Previous no-show history
- Booking lead time
- Reminder status
- Age group
- Appointment type
- Distance to clinic

These areas are being investigated to determine which findings have the greatest relevance for HealthConnect decision-making and potential modelling.

### Business impact

The Week 6 analysis focuses on identifying findings with the greatest potential operational impact for HealthConnect.

The analysis is intended to support practical decisions around appointment management, reminder processes, patient segmentation and administrative follow-up.

Recommendations are based on observed patterns and are not presented as causal conclusions.

### Cross-track contribution — Data Science

The Data Analytics track collaborated with the Data Science track by providing analytical findings relevant to feature investigation and modelling decisions.

Key analytical areas shared include:

- Previous no-show history
- Booking lead time
- Reminder status
- Appointment type
- Distance to clinic
- Age group

The purpose of the collaboration is to help Data Science evaluate whether analytically relevant variables should be investigated during feature refinement and model development.

Any modelling use of these variables should also consider whether the information would be available at the intended prediction point.

### Data limitations

The HealthConnect dataset is fictional/synthetic.

The analysis remains observational and does not establish causality.

Some analytical segments may contain fewer observations than others, which can affect the reliability of comparisons between groups.

The relatively small number of appointments in the 30+ km distance group is an important consideration when interpreting the distance-related finding.

Variables should also be evaluated based on whether they would be available at the intended prediction point before being considered for modelling.

### Week 7 analytical testing requirements

Week 7 will focus on testing and refining the Week 6 analytical findings.

Planned areas include:

- Testing the stability of key findings
- Reviewing unresolved analytical questions
- Validating integrated analytical and modelling outputs
- Assessing whether identified analytical features improve model development
- Refining dashboard insights based on testing results

### Week 6 progression

Week 5:
Initial EDA → KPI development → Initial dashboard → Business insights

Week 6:
Deeper analysis → KPI validation → Dashboard improvement → Cross-track integration → Decision support

Week 7:
Testing → Refinement → End-to-end validation
