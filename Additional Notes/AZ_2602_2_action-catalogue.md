# AZ_2602_2 — DPA action catalogue from validation exercise

Items where DPA model/analysis work has been surfaced by the external validation. Grouped by scope status so it's clear what bills against the current workstream, what needs a scope conversation with AZ, and what's future-phase.

For all items: surface to Darren before committing externally, and use yes-and framing when proposing the not-in-scope ones to AZ.

---

## A. In-scope — part of finalising the current report

These bill against AZ_2602_2 External Validation as-is. They're closing out the existing deliverable.

| # | Item | Owner | Notes |
|---|---|---|---|
| A1 | Williamson Results section: replace the "tracks worst-case intensive arm / pseudo-CI" framing | Sulayman draft + Darren review | Conflicts with Jieling's "compare to standard arm only" steer |
| A2 | Verify naive vs baseline-adjusted dementia curve ordering against the master plot | Darren | Jieling flags it looks reversed (SPRINT 140 vs BAX 150 should put naive below, not above) |
| A3 | Verify micro/normo/macro ordering on Figure 5 against the master plot | Darren | Visible clustering in the figure; may be a real null-signal artefact or a plotting bug |
| A4 | Verify top-panel label on the eGFR-decline/ESKD figure | Sulayman | Jieling's "should this be CV events?" — quick check |
| A5 | Fix duplicate Figure 6 (BPLTTC figure → Figure 7) and broken "Figure 4 below" → "Figures 5 and 6 below" reference in Binding section | Sulayman | Editorial |
| A6 | Strip three "DB note to AZ team" placeholders | Sulayman | Editorial |
| A7 | Reconcile prose vs Table 3 numbers (Ettehad) and Table 4 N (1M vs 5M) vs Simulation settings | Sulayman + Darren | Spot-check per QA |
| A8 | Add missing references (Go, Grams, Nelson, SCORE2, Cardoso, Yang, Reboussin, Pankratz, Anaturk, Roberts) | Sulayman | Bibliographic |
| A9 | Competing-risks sanity check on the Binding HR systematic skew below 1 | Darren | Quick check — table 4 HRs all sit below 1 across MACE/HF, which is more than noise; likely competing risks but worth confirming |

---

## B. Borderline — confirm with Darren whether in-scope or needs AZ scope conversation

| # | Item | What it produces | Decision needed |
|---|---|---|---|
| B1 | **HF input swap: Cardoso → Yang et al. (RR=0.82) in base case** | Model re-run; updated Table 3 + Figure 3; updated Ettehad Discussion text; potential downstream ICER change | Base-case model change driven *by* the validation. Could be argued as "addressing validation findings" (in-scope) or as a model amendment (new scope). Confirm with Darren, then AZ. ⚠️ Also confirm the "more conservative" wording with Jieling before writing as done. |
| B2 | Williamson re-plot against SPRINT-MIND standard arm only (drop intensive arm comparison) | Regenerated Figure 2; updated Results text | Smallish. If it's just a re-plot to align with Jieling's steer, arguably in-scope under A1. If it triggers re-interpretation of the comparison, bigger. |

---

## C. Clear new scope — propose to AZ as yes-and follow-up

These were surfaced *by* the validation but are new analytical work. Frame as a follow-up scenario set rather than absorbing silently. The existing Conclusion next-steps already gestures at C3 and C4 — that doesn't make them in-scope, just pre-flagged.

| # | Item | What it produces | Sizing flag |
|---|---|---|---|
| C1 | All-CKD or all-T2D baseline scenario for Binding absolute-risk comparison | Model run with modified baseline cohort; regenerated Figures 5 & 6 for the scenario; commentary showing the eGFR slope is recovered when SCORE2-CKD/SCORE2-Diabetes kick in | Single confirmatory scenario, modest |
| C2 | %CKD comparison across naive run, baseline-adjusted run, and Binding cohort | Quantification of how much of the macroalbuminuria HR gap is attributable to baseline CKD % | Small extraction + comparison |
| C3 | Targeted age-attenuation scenario analysis (BPLTTC finding) | Scenario(s) bounding the impact of the missing age-attenuation effect under different baseline age distributions | Moderate — depends on whether it's a sensitivity on age distribution or a synthetic age-attenuation factor applied to results |
| C4 | Goodness-of-Fit framework (MAPE, 45-degree identity lines) | Standardised performance metrics across the five validation comparisons, comparable to HEOR tech report rigour | Moderate analytical workstream |
| C5 | Estimate HR of SBP reduction on dementia from simulated output | Quantification of the dementia benefit the model currently imposes; supports the Williamson Discussion claim | Small — analytical extraction from existing runs |

**Yes-and framing for AZ:** "Yes, we can run these — they'd sit as a short follow-up scenario set, either against an extension to AZ_2602_2 or a separate workstream. Happy to scope effort once you confirm which to prioritise."

---

## D. Future phase — model development, not validation

Likely a separate engagement or a future model-version release. Catalogue here so they're not lost.

| # | Item | What it would involve |
|---|---|---|
| D1 | Incorporate age-attenuation of the SBP-reduction benefit into the model | Structural model change to risk equations; Conclusion already flags as model-dev item |
| D2 | MCI + Dementia consistent UKBDRS specification | Model variant where both risk equations come from UKBDRS rather than mixing UKBDRS and Mayo |
| D3 | Address direct treatment effect on eGFR decline | Pending ARTIC/PACIFIC long-term clinical data (already flagged in Thomas Discussion + Conclusion) |
| D4 | Add an eGFR risk modifier (parallel to existing uACR risk modifier) | Would let SCORE2-driven absolute risk slope with baseline eGFR for non-CKD/non-T2D patients |

---

## E. Data ask to AZ

| # | Item | Notes |
|---|---|---|
| E1 | Baseline MCI prevalence in BAX trial cohort | Currently assumed zero in the simulation; under-predicts baseline dementia risk. Worth asking AZ whether trial data captures this |

---

## F. Open questions for Jieling (must close before report goes final)

| # | Item |
|---|---|
| F1 | "More conservative" framing for Yang RR=0.82 — confirm intended sense (the ICER direction is ambiguous as written) |
| F2 | UKBDRS/Mayo source mapping — her email prose and table contradict each other on which equation applies to MCI-history vs no-MCI patients |
| F3 | Top-panel figure label (covered under A4) |

---

## Suggested workflow

1. Walk Darren through this list at the next internal sync. Get his read on B1 and B2 (in-scope vs new) and his sizing on C1–C5.
2. Close F1–F3 with Jieling alongside or before the next AZ catchup.
3. Once Darren has sized C1–C5, draft a yes-and email to AZ proposing a follow-up scenario package — let them prioritise.
4. A–E items get logged in the project tracker with the appropriate workstream allocation. Don't let any of B1, B2, or the C-items silently absorb against AZ_2602_2 without a scope-adjustment conversation.
