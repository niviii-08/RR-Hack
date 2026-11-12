# Rajasthan Royals · SupeRR Selector Season 2 (Round 1)
### Identifying the Most Reliable Players Under Pressure for the IPL 2027 Auction

![Vercel Live Dashboard](https://img.shields.io/badge/Vercel-Live_Dashboard-EA1A85?style=for-the-badge&logo=vercel)
![Deliveries](https://img.shields.io/badge/Deliveries_Modeled-200%2C961-182449?style=for-the-badge)
![Matches](https://img.shields.io/badge/Matches-867-254AA5?style=for-the-badge)
![CV Proof](https://img.shields.io/badge/Out--of--Sample_CV-r_%3D_0.6242-0D9488?style=for-the-badge)

An advanced sports analytics pipeline and integer-optimized franchise war-room system built for **Rajasthan Royals' SupeRR Selector Season 2**.

---

## 🚀 Live Interactive War-Room Dashboard
Access the interactive dashboard directly in your browser:
* **Interactive Model Tuner:** Drag sliders for HP Output, Uplift, and Consistency to recalculate rankings in real time.
* **Head-to-Head Radar Comparison:** Compare any two players across 6 clutch dimensions.
* **Rajasthan Royals 2027 MILP XI Solver:** View the mathematically optimized Playing XI and ₹52 Cr auction knapsack solution.
* **Download Full Methodology Report:** Direct download of the 7-page executive PDF report.

---

## 🏆 Final Locked Rankings (Unstop Dropdowns)

| Rank | Top 10 Batters Under Pressure | Top 10 Bowlers Under Pressure |
|:---:|---|---|
| **1** | **Suryakumar Yadav** (PRS 86.2) | **Sunil Narine** (PRS 94.8) |
| **2** | **Shreyas Iyer** (PRS 84.8) | **Adam Zampa** (PRS 86.2) |
| **3** | **Tristan Stubbs** (PRS 84.6) | **Jasprit Bumrah** (PRS 85.0) |
| **4** | **Shashank Singh** (PRS 80.3) | **Mitchell Starc** (PRS 83.4) |
| **5** | **Namboori Tilak Varma** (PRS 79.9) | **Gudakesh Motie** (PRS 82.7) |
| **6** | **Rajat Patidar** (PRS 76.3) | **Mohammad Nawaz** (PRS 81.2) |
| **7** | **Harry Brook** (PRS 75.5) | **Shaheen Afridi** (PRS 79.8) |
| **8** | **Heinrich Klaasen** (PRS 75.0) | **Kuldeep Yadav** (PRS 79.3) |
| **9** | **Tim David** (PRS 75.0) | **Abrar Ahmed** (PRS 78.7) |
| **10** | **Andre Russell** (PRS 74.4) | **Mitchell Santner** (PRS 78.6) |

---

## 🧠 Key Methodology Highlights

1. **4-Pillar Win-Probability Leverage Index ($P_i \in [0, 100]$):**
   - Pre-delivery logistic models ($82.2\%$ Inn 2, $64.1\%$ Inn 1 accuracy) capture contest closeness, scoring urgency, and collapse stress.
   - Proved that high-pressure deliveries trigger a **2.0× surge in wicket rates** ($4.74\% \to 9.54\%$) and spike chase run rates above 10 RPO.
2. **Solving the Negative-Baseline Trap:**
   - Implemented **Floored Baseline Uplift**: $\text{Uplift} = \text{HP} - \max(\text{LP}, 0)$, ensuring always-elite stars (Heinrich Klaasen, Tim David) aren't penalized over players with poor routine baselines.
3. **Out-of-Sample Cross-Validation ($r = 0.6242$):**
   - Grid search trained on 2022–2024 and tested on 2025–2026 crunch matches mathematically proved the optimal weighting function ($50\%$ HP, $25\%$ Uplift, $15\%$ Match Rate, $10\%$ Sharpe).
4. **Rajasthan Royals MILP Auction Knapsack Optimizer:**
   - Addressed RR's specific **$-35.94$ Death Bowling gap** and **$-7.08$ Death Batting gap**.
   - Solved standard ₹120 Cr IPL purse limits with ₹52 Cr remaining auction capital to acquire **Tristan Stubbs**, **Gudakesh Motie**, **Adam Zampa**, and **T Natarajan**.

---

## 📁 Repository Structure
* `index.html` — Interactive Single-Page Dashboard (Chart.js + Dynamic Sliders).
* `report.pdf` — Complete 7-Page Executive Methodology Report (PDF).
* `charts/` — 300-DPI publication charts (Dumbbell plots, Quadrants, Bootstrap CIs, RR Gaps).

---
*Created for Rajasthan Royals · SupeRR Selector Season 2.*
