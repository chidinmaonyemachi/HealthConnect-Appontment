# HealthConnect Clinic Experience Lab

## Exploratory Analysis, KPI Development & Business Insights

### Project objective
The analysis prepares the appointment dataset, investigates attendance and no-show patterns, calculates selected KPIs, develops an initial analytical dashboard, and translates the results into business insights and recommendations.

### Project resources
- HealthConnect Appointment Dataset
- HealthConnect Data Dictionary
- AnalystLab Africa Guide

### Dataset overview
- 5,000 appointment records
- 18 original variables
- 5,000 unique appointment IDs
- 1,696 unique patients
- Appointment period: 2025-01-01 to 2026-06-30
- Final outcomes: Attended, No-Show, Cancelled

### Data preparation
- Original project resources preserved without overwrite
- Data types validated and dates converted appropriately
- 0 exact duplicate rows
- 90 missing `distance_to_clinic_km` values (1.8%) retained as missing
- 60 missing `waiting_time_minutes` values (1.2%) retained as missing
- No date, booking-lead, appointment-day, age-group, history, or reminder-channel consistency errors detected
- Derived analytical fields created for appointment month, booking lead-time band, previous no-show group, distance band and waiting-time band

### Selected KPIs
| KPI | Result |
|---|---:|
| No-Show Rate | 48.46% |
| Total Attendance | 5,000 |
| Total Cancellation | 263 |
| Reminder Coverage Rate | 72.68% |
| Avg Booking lead days | 29.64|


### Key findings
1. Booking lead time shows the strongest initial pattern: no-show rate rises from 27.81% for appointments booked 0-7 days ahead (short notice) to 53.82% for appointments booked 46-60 days ahead (1-1.5 months).
2. Previous no-show history is strongly associated with current no-show behaviour: 46.30% with no previous no-shows versus 70.33% with three or more.
3. Appointments with reminders have a lower observed no-show rate (47.36%) than appointments without reminders (51.39%). This is an association, not proof of causation.
4. No-show rates generally increase with distance from the clinic, reaching 52.91% for 16-30 km and 68.06% for the 30+ km group. The 30+ km group is small (72 appointments), so the result should be interpreted cautiously.
5. Follow-up appointments have the highest observed no-show rate among appointment types at 51.23%.
6. Waiting time, age group, appointment day and appointment time show smaller differences than booking lead time and previous no-show history.

### Business recommendations
- Prioritise long-lead appointments for proactive confirmation or enhanced reminder workflows.
- Use previous no-show history as a segmentation factor for targeted administrative follow-up.
- Review why 51.39% of appointments did not receive a reminder and assess whether coverage can be improved.
- Investigate reminder-channel performance further before attributing lower no-show rates to a specific channel.
- Consider additional administrative support for longer-distance patients, subject to further analysis and clinic policy.
- Review follow-up appointment workflows because this appointment type has the highest observed no-show rate.

### Important limitation
The HealthConnect dataset is fictional/synthetic. The analysis is exploratory and observational. Reported relationships should be described as associations and should not be presented as causal evidence.


