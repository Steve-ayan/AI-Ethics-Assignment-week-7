# 🌟 AI Ethics Audit: Designing Responsible and Fair Systems

## Author: Stephen Ayankoso ✍️
---

## 🛡️ 1. Project Overview & Objective

* **Theme:** Designing Responsible and Fair AI Systems
* **Context:** Week 7 PLP Program Assignment
* **Objective:** To evaluate the fairness of the **COMPAS Recidivism Dataset** using the AI Fairness 360 (AIF360) toolkit, analyze high-stakes bias case studies, and propose ethical governance policies.

---

## 🔎 2. Key Audit Findings (COMPAS Dataset)

*This section summarizes the results from the **Part 3: Practical Audit**.*

The audit of the raw dataset labels confirmed significant pre-existing disparity against the African-American (Unprivileged) group regarding the **Favorable Outcome (Non-Recidivism)**.

| Metric | Unprivileged Group (AA) | Privileged Group (Caucasian) | Disparity | Interpretation |
| :--- | :--- | :--- | :--- | :--- |
| **Favorable Outcome Rate (P(Y=0))** | **0.4857** | **0.6064** | 0.1207 | AA defendants have a 12% lower chance of having a 'favorable' outcome in the dataset. |
| **Disparate Impact Ratio (DIR)** | N/A | N/A | **0.8009** | **On the threshold (0.80) of severe adverse impact.** |

**Conclusion:** The DIR of 0.8009 validates the presence of systemic bias in the data used to train the COMPAS tool, confirming that the Unprivileged group receives the favorable outcome at only 80% the rate of the Privileged group.

---

## 📁 3. Deliverables and Contents

| File/Section | Assignment Part | Description |
| :--- | :--- | :--- |
| **part1\_theory\_answers.md** | Part 1 (30%) | Definitions of bias, transparency vs. explainability, and GDPR impact. |
| **part2\_case\_studies.md** | Part 2 (40%) | Analysis and remediation proposals for the Biased Hiring Tool and Facial Recognition cases. |
| **part3\_audit\_report.md** | Part 3 (25%) | 300-word summary of the audit findings, remediation steps, and FPR disparity. |
| **part3\_practical\_audit.ipynb** | Part 3 (25%) | Working Python code for data loading, preprocessing, and metric calculation (DIR). |
| **part4\_ethical\_reflection.md** | Part 4 (5%) | Reflection on ethical adherence for a Predictive Maintenance Model (Civil Engineering Focus). |
| **bonus\_ai\_healthcare\_policy.md** | Bonus Task (10%) | 1-page guideline for ethical AI use in healthcare (Consent, Bias, Transparency). |

---

## ⚖️ 4. Ethical Policy Highlights

The project’s proposals consistently adhere to:

* **Justice:** Mitigating bias using **Reweighting** (Part 3) and ensuring resources are not under-allocated in vulnerable areas (Part 4).
* **Non-maleficence:** Prioritizing the minimization of False Negatives (FN) in high-stakes systems (Part 4) to prevent physical or systemic harm.
* **Transparency/Autonomy:** Mandating **SHAP values** for model explanations (Part 4) and implementing a **Layered Consent Protocol** with a "Right to Human Review" in the healthcare policy (Bonus Task).

***
