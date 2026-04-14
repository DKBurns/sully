
# Scoping Review Report: External Validation Sources for HTN Microsimulation Model
## 1. Overview
This report summarises findings from 6 known source papers and their bibliographies, assessed for relevance to external validation of a hypertension (HTN) cost-effectiveness microsimulation model. The model tracks CVD events (MI, UA, stroke, TIA, HF), CKD progression (stages 3a–5, ESRD, transplant), cognitive decline (MCI, dementia), diabetic retinopathy, and mortality (CV/non-CV). It uses modern risk equations (SCORE2-family, SMART2, PREVENT, CKDPC, KFRE, Mayo cognitive, UKBDRS, Gallego/Cugati) and outputs SBP/eGFR/uACR trajectories, QALYs, costs, life years, and survival.
---
## 2. Paper Summaries
### 2.1 Wu et al. (2021) — BMJ Open
- **DOI:** `10.1136/bmjopen-2021-052884`
- **Title:** Gaps in antihypertensive and statin treatments and benefits of optimisation
- **Model:** Markov (HPS-CVD policy model), parametric survival for CVD endpoints
- **Population:** 91,828 HTN + 23,723 CVD patients, east London, ethnically diverse (35% white, 31% South Asian, 26% black)
- **Intervention:** Antihypertensive/statin treatment optimisation vs current care
- **Perspective/Horizon:** UK NHS / Lifetime
- **Risk equations:** HPS-CVD model, QRISK3 (ethnicity HR adjustment), BP Trialists' Collaboration meta-analysis HRs, CTT Collaboration (statins), EQ-5D (Dolan 1997)
- **Key outputs:** Composite MVE/OVE rates per 1000 patients (5yr/10yr/lifetime), vascular deaths avoided, QALYs by age group (0.31–1.11), life years by age group (0.54–1.36), hospital cost savings (~£1,100/person net)
### 2.2 Sharp et al. (2024) — EHJQCCO
- **DOI:** `10.1093/ehjqcco/qcae001`
- **Title:** Cost-effectiveness of catheter-based RF renal denervation for uncontrolled HTN (UK)
- **Model:** Markov (33 states, 1-month cycle, half-cycle correction)
- **Population:** SPYRAL HTN-ON MED (n=337), mean age 55, 19.9% female, baseline oSBP 163 mmHg
- **Intervention:** RF RDN (Symplicity SPYRAL) vs sham
- **Perspective/Horizon:** UK NHS / Lifetime
- **Risk equations:** Framingham (stroke, CHD, HF), PROCAM (MI), NHANES (ESRD), Thomopoulos meta-regression (RR per SBP), QRISK3 (validation only)
- **Key outputs:** Cumulative event rates at 10yr (stroke 9.0%, MI 7.5%, HF 5.0%, ESRD 0.40%, CVD death 4.9%), RRs by event, QALYs (13.40 vs 13.76), ICER £13,482/QALY, utility values by state (stroke 0.63, MI 0.76/0.88, HF 0.68, ESRD 0.72)
### 2.3 Geisler et al. (2012) — JACC
- **DOI:** `10.1016/j.jacc.2012.07.029`
- **Title:** Cost-effectiveness of catheter-based renal denervation for resistant HTN
- **Model:** Markov (7 states, 1-year cycle)
- **Population:** Symplicity HTN-2, mean age ~58, baseline SBP 178 mmHg, resistant HTN
- **Intervention:** RDN vs SoC
- **Perspective/Horizon:** US societal / Lifetime
- **Risk equations:** Framingham (stroke, CHD, HF), MRFIT (ESRD/renal decline), US life tables
- **Key outputs:** 10yr RRs (stroke 0.70, MI 0.68, CHD 0.78, HF 0.79, ESRD 0.72), median survival 18.4 vs 17.1 yr, ICER $3,071/QALY, EQ-5D utilities (Sullivan & Ghushchyan 2006)
### 2.4 Taylor et al. (2024) — PharmacoEconomics Open
- **DOI:** `10.1007/s41669-024-00472-z`
- **Title:** Cost effectiveness of endovascular ultrasound renal denervation in resistant HTN
- **Model:** Markov (11 states, 1-month cycle, half-cycle correction)
- **Population:** RADIANCE-HTN TRIO (n=136), baseline oSBP 155.3 mmHg
- **Intervention:** Ultrasound RDN (Paradise) vs SoC
- **Perspective/Horizon:** UK NHS / Lifetime
- **Risk equations:** Framingham + PROCAM (baseline risk), Thomopoulos (base case RR), Ettehad (scenario), Rahimi (scenario), QRISK3 (validation), Khan (HF)
- **Key outputs:** LYs 15.14 vs 14.37, QALYs 12.12 vs 11.49, ICER £5,600/QALY, SBP reduction −8.5 mmHg, ABPM −8.0 mmHg median
### 2.5 Constanti et al. (2021) — Hypertension
- **DOI:** `10.1161/HYPERTENSIONAHA.120.14913`
- **Title:** Cost-effectiveness of initiating treatment in stage 1 HTN based on 10-year CVD risk
- **Model:** Markov (1-year cycle, lifetime, up to 60 cycles)
- **Population:** Stage 1 HTN (SBP 140–159), no CVD/CKD/DM, ages 40–75
- **Intervention:** Antihypertensive drug vs none
- **Perspective/Horizon:** UK NHS / Lifetime
- **Risk equations:** QRISK2/QRISK3 (threshold determination), Brunström & Carlberg meta-analysis (treatment RRs), Law et al. (age adjustment), EQ-5D (Sullivan 2011 / HSE 2014)
- **Key outputs:** ICER £10,017/QALY (men, 10% risk) and £8,635/QALY (women, 10% risk), CVD events modelled: MI, stroke, HF, TIA, stable angina, unstable angina, NNT 5–136 by sex
### 2.6 Smith & Campbell (2013) — AJH
- **DOI:** `10.1093/ajh/hpt099`
- **Title:** Cost-effectiveness of renin-guided treatment of hypertension
- **Model:** Markov (state-transition)
- **Population:** Treated uncontrolled HTN, males age 63
- **Intervention:** PRA-guided therapy vs standard care
- **Perspective/Horizon:** US / Lifetime
- **Risk equations:** Framingham (CHD: Anderson 1991, stroke: D'Agostino 1994, HF: Kannel 1999), Hsu (ESRD), US life tables, EQ-5D (Sullivan & Ghushchyan 2006)
- **Key outputs:** QALYs 12.727 vs 12.618, costs $23,648 vs $22,077, ICER $14,497/QALY
---
## 3. Endpoint Comparison Matrix
Mapping of model endpoints against what each paper reports.
| Endpoint | Wu (2021) | Sharp (2024) | Geisler (2012) | Taylor (2024) | Constanti (2021) | Smith (2013) |
|---|---|---|---|---|---|---|
| SBP over time (office) | Baseline only | Reductions reported | −32 mmHg | −8.5 mmHg | No (risk categories) | Baseline input |
| SBP over time (ambulatory) | No | No | No | −8.0 mmHg median | No | No |
| eGFR decline (CKD) | No | No | No | No | No | No |
| eGFR decline (non-CKD) | No | No | No | No | No | No |
| uACR progression | No | No | No | No | No | No |
| MI incidence (primary) | Composite MVE | **Yes** (7.5% 10yr) | **Yes** (RR 0.68) | **Yes** | **Yes** | **Yes** |
| MI incidence (secondary) | No | No | No | No | No | No |
| Unstable angina incidence | No | **Yes** | No | No | **Yes** | No |
| Stroke incidence | Composite MVE | **Yes** (9.0% 10yr) | **Yes** (RR 0.70) | **Yes** | **Yes** | **Yes** |
| TIA incidence | No | No | No | No | **Yes** | No |
| Heart failure incidence | Composite OVE | **Yes** (5.0% 10yr) | **Yes** (RR 0.79) | **Yes** | **Yes** | **Yes** |
| CVD case fatality | Vascular deaths | **Yes** (4.9% 10yr) | Included | Included | CVD death modelled | Included |
| CVD event composition | MVE/OVE split | **Yes** (full split) | **Yes** (full split) | **Yes** (full split) | **Yes** (6 types) | MI/stroke/HF |
| CKD stage 3a incidence | No | No | No | No | No | No |
| ESRD incidence | No | **Yes** (0.40% 10yr) | **Yes** (RR 0.72) | **Yes** | No | No |
| Kidney transplant | No | No | No | No | No | No |
| MCI incidence | No | No | No | No | No | No |
| Dementia incidence | No | No | No | No | No | No |
| Diabetic retinopathy | No | No | No | No | No | No |
| CV death | **Yes** | **Yes** | **Yes** | **Yes** | **Yes** | **Yes** |
| Non-CV death | **Yes** | **Yes** | **Yes** | **Yes** | **Yes** | **Yes** |
| Overall survival / LYs | **Yes** (by age) | Implied | **Yes** (18.4 vs 17.1) | **Yes** (15.1 vs 14.4) | No explicit LYs | No explicit LYs |
| Event-free survival (KM) | No | No | No | No | No | No |
| Baseline utility | **Yes** (EQ-5D) | **Yes** (state-specific) | **Yes** (EQ-5D) | **Yes** (state-specific) | **Yes** (EQ-5D) | **Yes** (EQ-5D) |
| Total discounted QALYs | **Yes** (by age) | **Yes** (13.40/13.76) | **Yes** (implied) | **Yes** (12.12/11.49) | **Yes** (via ICER) | **Yes** (12.73/12.62) |
| Life years by health state | **Yes** (by age) | Implied | Median survival | **Yes** (by arm) | No | No |
| Treatment discontinuation | No | No | No | No | Adherence discussed | No |
---
## 4. Risk Equation Comparison Matrix
Mapping of risk equations used in the model against those used in each paper.
| Risk Equation (Model) | Wu (2021) | Sharp (2024) | Geisler (2012) | Taylor (2024) | Constanti (2021) | Smith (2013) |
|---|---|---|---|---|---|---|
| SCORE2 | — | — | — | — | — | — |
| SCORE2-OP | — | — | — | — | — | — |
| SCORE2-Diabetes | — | — | — | — | — | — |
| SCORE2-CKD | — | — | — | — | — | — |
| PREVENT (ASCVD) | — | — | — | — | — | — |
| PREVENT (HF) | — | — | — | — | — | — |
| SMART2 | — | — | — | — | — | — |
| Framingham Recurrent CHD | — | **Yes** | **Yes** | **Yes** | — | **Yes** |
| CKDPC (60/45/30) | — | — | — | — | — | — |
| KFRE | — | — | — | — | — | — |
| Mayo MCI | — | — | — | — | — | — |
| Mayo Dementia | — | — | — | — | — | — |
| UKBDRS | — | — | — | — | — | — |
| Gallego/Cugati (DR) | — | — | — | — | — | — |
| Baseline utility eqs | HPS/Dolan | Ward/Henry/Comin-Colet | Sullivan | Published | Sullivan/HSE | Sullivan |
**Other equations used in papers (not in model):**
| Equation | Papers |
|---|---|
| HPS-CVD policy model | Wu (2021) |
| QRISK3 (HR adjustment / validation) | Wu (2021), Sharp (2024), Taylor (2024), Constanti (2021) |
| PROCAM (MI risk) | Sharp (2024), Taylor (2024) |
| NHANES / MRFIT (ESRD) | Sharp (2024), Geisler (2012), Smith (2013) |
| Thomopoulos meta-regression (RR per SBP) | Sharp (2024), Taylor (2024) |
| Ettehad meta-analysis (RR per SBP) | Taylor (2024) |
| Rahimi IPD meta-analysis (HR per SBP) | Taylor (2024) |
| Brunström & Carlberg (treatment RRs) | Constanti (2021) |
| Khan 10-yr HF risk | Taylor (2024) |
---
## 5. Bibliography Snowball — Candidate Studies for Validation
References cited across the 6 papers that may provide external validation data for specific model endpoints.
### 5.1 CVD Incidence and Event Composition
| Reference | Cited In | Potential Validation Use |
|---|---|---|
| Rapsomaniki et al. (2014) Lancet 383:1899 — BP and incidence of 12 CV diseases in 1.25M people | Sharp | Lifetime CVD risks by BP level, event composition by age/sex |
| Asaria et al. (2017) Lancet Public Health 2:e191 — MI admissions and deaths in England | Sharp | MI incidence and case fatality rates, England |
| Smolina et al. (2012) Circ CQO 5:532 — Long-term MI survival and recurrence, England 2004–2010 | Sharp | Post-MI survival, recurrence rates |
| Cowie et al. (1999) EHJ 20:421 — HF incidence and aetiology, population-based | Constanti | HF incidence rates |
| Velagaleti et al. (2008) Circulation 118:2057 — HF incidence trends post-MI | Sharp | HF after MI (secondary prevention) |
| Seshadri et al. (2006) Stroke 37:345 — Lifetime risk of stroke, Framingham | Sharp | Lifetime stroke risk by age/sex |
| Huffman et al. (2013) JACC 61:1510 — Lifetime risk of HF | Sharp | Lifetime HF risk by race/sex |
| Wafa et al. (2020) PLoS Med 17:e1003048 — Long-term stroke outcomes, South London | Sharp | Post-stroke mortality and dependence over time |
| Herrett et al. (2019) Lancet 394:663 — CVD burden by BP lowering strategy | Constanti | CVD event rates by treatment strategy |
### 5.2 CKD and Renal Endpoints
| Reference | Cited In | Potential Validation Use |
|---|---|---|
| Turin et al. (2012) JASN 23:1569 — Lifetime risk of ESRD | Sharp | Lifetime ESRD risk — validation target |
| Hsu et al. (2004) Ann Intern Med 141:95 — ESRD incidence by CKD stage | Sharp | ESRD incidence rates by eGFR |
| Walker et al. (1992) JAMA 268:3085 — MRFIT renal function change by BP | Geisler | eGFR decline rate by SBP level |
| UK Renal Registry 24th Annual Report (2022) | Sharp | ESRD/RRT incidence, prevalence, survival in UK |
| Li et al. (2015) NDT 30:1726 — Cost of renal replacement therapy | Sharp | RRT costs for UK validation |
### 5.3 Cognitive Decline
| Reference | Cited In | Potential Validation Use |
|---|---|---|
| Williamson et al. (2019) JAMA 321:553 — SPRINT MIND, intensive BP and dementia | Constanti | BP lowering effect on probable dementia incidence |
| Lennon et al. (2019) JAD 71:307 — Midlife HTN and Alzheimer's meta-analysis | Constanti | HTN-dementia risk association, meta-analytic HRs |
### 5.4 Treatment Effects and SBP Reduction
| Reference | Cited In | Potential Validation Use |
|---|---|---|
| Thomopoulos et al. (2014) J Hypertens 32:2285 — Meta-analysis of BP lowering on outcomes | Sharp, Taylor | RR per 10 mmHg SBP for stroke/CHD/HF/mortality |
| Ettehad et al. (2016) Lancet 387:957 — BP lowering and CVD prevention | Taylor | Alternative RR estimates per 10 mmHg SBP |
| Rahimi et al. (2021) Lancet 397:1625 — IPD meta-analysis of BP lowering | Taylor | HR by baseline SBP level, treatment effect heterogeneity |
| Brunström & Carlberg (2018) JAMA Intern Med 178:28 — BP lowering by baseline SBP | Constanti | RRs stratified by baseline SBP level |
| Law et al. (2009) BMJ 338:b1665 — 147 RCTs of BP lowering | Constanti | BP reduction by drug class, age-adjusted treatment effects |
| SPRINT (2015) NEJM 373:2103 — Intensive vs standard BP control | Sharp, Constanti | SBP trajectories over time, CVD events, mortality by target |
### 5.5 Risk Equation Validation / Cross-Comparison
| Reference | Cited In | Potential Validation Use |
|---|---|---|
| Hippisley-Cox et al. (2017) BMJ 357:j2099 — QRISK3 | Wu, Sharp, Taylor, Constanti | 10-yr CVD risk predictions for cross-validation vs SCORE2 |
| Khan et al. (2019) JACC 73:2388 — 10-year HF risk equations | Taylor | HF risk predictions for comparison with PREVENT(HF) |
### 5.6 Large HTN Outcome Trials (Event Rate Validation)
| Reference | Cited In | Potential Validation Use |
|---|---|---|
| ALLHAT (2002) JAMA 288:2981 | Geisler, Smith | CVD outcomes in high-risk HTN by drug class |
| ASCOT-BPLA (Dahlof 2005) Lancet 366:895 | Geisler, Smith | CVD outcomes, SBP trajectories |
| VALUE Trial (Julius 2004/2006) | Sharp | HTN trial CVD outcomes |
| ONTARGET (2008) NEJM 358:1547 | Sharp | CVD outcomes in high-risk, secondary prevention |
| TRANSCEND (2008) Lancet 372:1174 | Sharp | CVD in ACEi-intolerant patients |
| HOPE Study (2000) Lancet 355:253 | Sharp | CVD + renal outcomes in diabetic HTN |
| STEP Trial (Zhang 2021) NEJM 385:1268 | Sharp | Intensive BP in older patients, SBP trajectories |
### 5.7 Utility and Cost Inputs
| Reference | Cited In | Potential Validation Use |
|---|---|---|
| Sullivan & Ghushchyan (2006) Med Decis Making 26:410 | Geisler, Smith | EQ-5D utility values by chronic condition (US) |
| Sullivan et al. (2011) Med Decis Making 31:800 | Constanti | EQ-5D catalogue for UK |
| Ward et al. (2007) HTA 11:1-160 | Sharp | Utility values for CVD states |
| Gorodetskaya et al. (2005) Kidney Int 68:2801 | Sharp | ESRD utility (0.72) |
| Dolan (1997) Med Care 35:1095 | Wu | EQ-5D valuation tariff |
---
## 6. Key Gaps and Observations
### 6.1 No paper uses the model's core risk equations
None of the 6 papers use SCORE2, SCORE2-OP, SCORE2-CKD, SCORE2-Diabetes, PREVENT (ASCVD/HF), SMART2, CKDPC, KFRE, Mayo MCI/Dementia, UKBDRS, or Gallego/Cugati. All rely on Framingham-family equations. This makes direct structural validation difficult but enables cross-model comparison (same patients, different risk engines).
### 6.2 Major endpoint gaps across all 6 papers
No paper reports:
- eGFR trajectories over time (CKD or non-CKD)
- uACR progression
- CKD staging transitions (3a/3b/4/5)
- MCI or dementia incidence
- Diabetic retinopathy incidence
- Kidney transplant rates
- Event-free survival (Kaplan-Meier)
- MI incidence in secondary prevention specifically
- Treatment discontinuation rates
These gaps require **clinical cohort studies** (not CEA models) for validation. Candidate sources include the original derivation cohorts for the risk equations used in the model (e.g., CKD-PC consortium data, Mayo Clinic Alzheimer's Disease Research Center data, UK Biobank).
### 6.3 Best direct validation candidates
1. **Sharp (2024)** — most granular: cumulative event rates by type (stroke, MI, HF, ESRD) at 10yr and lifetime, state-specific utilities, CVD death rates
2. **Geisler (2012)** — CVD + ESRD relative risks at 10yr and lifetime, median survival
3. **Taylor (2024)** — similar UK Markov structure, ambulatory BP data, multiple meta-analytic RR sources
### 6.4 Most promising bibliography leads for filling gaps
- **CKD/Renal:** Walker (1992), Turin (2012), UK Renal Registry, Hsu (2004)
- **Cognitive:** SPRINT MIND (Williamson 2019), Lennon (2019)
- **CVD event rates:** Rapsomaniki (2014), Asaria (2017), SPRINT (2015)
- **Cross-validation of risk equations:** QRISK3 (Hippisley-Cox 2017), Khan HF (2019)
