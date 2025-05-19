
# Thesis Recovery Plan – Plant-Based Food Attitude Study (SOR Model with PLS-SEM)

---

## 1  Re-check the measurement model **before** touching the hypotheses  

> 70 – 80 % of “rejected” structural paths in honours-level theses trace back to weak measurement, not “bad theory”.

| Task | What to do | Benchmarks* |
|------|------------|-------------|
| **Internal consistency** | Cronbach’s α, Composite Reliability (ρ<sub>c</sub>) | ≥ 0.70 |
| **Indicator loadings** | Reflective items: outer loading ≥ 0.70.  Drop items < 0.40, or 0.40–0.70 if α ↑ clearly. | – |
| **Convergent validity** | AVE ≥ 0.50 | – |
| **Discriminant validity** | Fornell–Larcker √AVE > inter-construct correlations **and** HTMT < 0.85 | – |

\*Hair et al., 2022, _A Primer on PLS-SEM_.  

If any construct fails, fix it **first** (drop/reword items or merge highly-overlapping constructs) and re-run the model.  A clean outer model will sometimes turn “non-significant” paths into significant ones because the estimates become less noisy.

---

## 2  Re-estimate the structural model with adequate power  

1. **Sample size**  
   *Calculate post-hoc power:* use G*Power (f² from SmartPLS output) or Kock & Hadaya’s minimum‐R² heuristic.  
   *If power < 0.80* ➜ collect ~30–50 more responses or merge similar groups.

2. **Bootstrapping settings**  
   *SmartPLS:* 5000 subsamples, no sign changes, Bias-Corrected CI.  
   Check VIF < 5 to rule out multicollinearity.

3. **Report full effect metrics**  
   | Metric | If you get… | How to write it |
   |--------|-------------|-----------------|
   | R² | Attitude ≈ 0.52, PI ≈ 0.49 (your quick OLS shows this) | “explains a moderate share of the variance” |
   | f² | ≥ 0.02 small, ≥ 0.15 medium, ≥ 0.35 large | emphasise which stimuli really move the needle |
   | Q² (blindfolding) | > 0 | “predictive relevance confirmed” |

---

## 3  Deal with “rejected” hypotheses intelligently  

| Currently non-significant | Typical fix | How to position in the thesis |
|---------------------------|-------------|------------------------------|
| **H2** (Health → Attitude) | Health may act **directly** on Purchase Intention or be already internalised in Attitude.  Test a direct path HC → PI and compare AIC. | “Contrary to expectation, health consciousness affects purchase more directly than through attitude, echoing …” |
| **H10-1 / H10-2** (Self-efficacy moderations) | Mean-centre and create interaction terms properly; split sample (high vs low SE) and run **multi-group analysis** – the difference test is often more powerful than single-path moderation. | “No global moderation was detected, but MGA shows the Attitude → PI path is 22 % stronger for high-SE consumers.” |
| **Any mediation (H6–H9)** | Use **BC bootstrapped indirect effects**; report VAF; if indirect is ns, discuss why. Sometimes a partial mediation (direct + indirect both sig.) is more realistic. | “Attitude partially mediates EC → PI (VAF = 43 %). HC shows only a direct effect, suggesting …” |

---

## 4  Re-shape the story rather than forcing significance  

1. **Keep the framework** but re-label unsupported paths as exploratory findings or boundary conditions.  A thesis does **not** have to support all hypotheses to pass; it has to be rigorous and honest.  
2. **Emphasise what _is_ significant:**  
   * Consumer Identity and Social-Media Exposure are strong stimuli (β≈ 0.28–0.32, _p_<0.001).  
   * Attitude strongly drives Purchase Intention (β≈ 0.84, _p_<0.001).  
   * Self-efficacy has a solid **direct** effect on Intention even if moderation fails (β≈ 0.83, _p_<0.01).  
3. **Explain the nulls** with theory and context (e.g., Vietnamese Gen-Z may already assume plant-based foods are healthy, so health consciousness adds little incremental attitude boost).  
4. **Limitations & future work** – small sample, cross-sectional, self-report, cultural setting, etc.

---

## 5  Write-up template (chapters 4 & 5)

> **Results (Ch. 4)**  
> * Table 4.1: Outer-model diagnostics (α, ρ<sub>c</sub>, AVE, HTMT)  
> * Table 4.2: Path coefficients, t, p, f²  
> * Figure 4.1: Final PLS model with β and *significance stars*  
> * Table 4.3: Mediation & Moderation results (BC 95 % CI)  
>   
> **Discussion (Ch. 5)**  
> 1. **Key findings vs. hypotheses** (supported / partially / not supported)  
> 2. **Comparison with recent SOR research on plant-based foods** – e.g., [Thai consumers’ online PBF study](https://pmc.ncbi.nlm.nih.gov/articles/PMC11096942/) and [bibliometric SOR review](https://www.researchgate.net/publication/387980300_Bibliometric_Analysis_of_Stimulus-Organism-_Response_Theory_Past_Developments_Current_Applications_and_Future_Trends)  
> 3. **Managerial implications** – highlight social-media and identity cues, leverage self-efficacy messages.  
> 4. **Theoretical implications** – refine SOR in sustainable food context; health–attitude link is context-dependent.  
> 5. **Limitations & future agenda.**

---

## 6  Extra robustness checks (optional but earns marks)

* **Common-method bias:**  full-collinearity VIF < 3.3 or marker-variable test.  
* **Non-response bias:** early-vs-late t-test on key constructs.  
* **Alternative models:** TPB (Subjective Norm, PBC) or add Perceived Value; compare fit via SRMR (SmartPLS → model fit).  

---

## 7  Practical steps the student can do this week

| Day | Action |
|-----|--------|
| 1 | Clean dataset, remove bad responses, run measurement diagnostics. |
| 2 | Re-specify model (drop/load items), run bootstrapping 5000 resamples. |
| 3 | Conduct mediation & moderation with bias-corrected CIs; run MGA if interactions still ns. |
| 4 | Draft Chapter 4 tables & figures; send to supervisor for quick feedback. |
| 5 | Write Discussion section; integrate literature (2023-2024 SOR & plant-based food papers). |
| 6 | Polish implications, limitations, power analysis appendix. |
| 7 | Full read-through, update abstract, compile references. |

---

### Remember  
*Your thesis is judged on methodological rigour and the ability to interpret results, not on getting “all paths significant”.*  A transparent report of why certain hypotheses failed—and what that tells future researchers—is often seen as more scholarly than a “perfect” model that hides non-significant findings.
