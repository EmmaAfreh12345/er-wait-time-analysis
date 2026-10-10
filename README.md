# ER Wait Time & Patient Flow Analysis

Python analysis of 10,000+ emergency room visits (Jan 2025 - Aug 2026), looking at where patients wait longest and what it costs in patient safety and hospital capacity.

**Tools:** Python, pandas, matplotlib, Jupyter Notebook

**Notebook:** [er_analysis.ipynb](er_analysis.ipynb)

## Business Questions

1. How does wait time change with patient acuity (ESI level)?
2. Do time of day and season affect waits?
3. What share of patients leave without being seen (LWBS), and is it linked to long waits?
4. How long do admitted patients board while waiting for an inpatient bed?
5. How long does each type of patient stay in the ER overall?

## Key Findings

- **Wait time rises sharply as acuity drops:** about 6 minutes (ESI 1) to about 162 minutes (ESI 5).
- **Evening and winter are the pressure points:** waits are about 40% longer from 6pm to 11pm and about 29% longer in winter.
- **Long waits drive patients away:** 11.3% of visits ended in LWBS. Among low-acuity patients, those who left had waited about 145 minutes, compared with about 122 minutes for those discharged.
- **Boarding nearly doubles in winter:** about 90 minutes outside winter versus about 179 minutes in winter.
- **Admitted patients stay longest:** about 200 minutes in the ER versus about 139 for discharged patients.

## Recommendations

- Add ER staffing during the 6pm-11pm window.
- Plan winter surge capacity for inpatient beds to reduce boarding.
- Track the LWBS rate among ESI 4-5 patients as a patient-safety metric.

## Skills Demonstrated

- Loading and inspecting data, with data-quality checks
- Date-time handling and derived columns in pandas
- Grouping, filtering and aggregating to answer business questions
- Visualization with matplotlib
- Turning results into business recommendations

## Files

- `er_analysis.ipynb`: full analysis with code, charts and findings
- `er_visits_raw.csv`: dataset used in the analysis
