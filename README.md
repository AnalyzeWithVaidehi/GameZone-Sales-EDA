# 📊 GameZone Exploratory Data Analysis (EDA): Uncovering Global Sales Trends & Product Anomalies

---

## 👋 Meet the Analyst

**Hi, I'm Vaidehi!** I am a Data Analyst specializing in transforming raw data pipelines into clear, actionable business strategies. With a background in computer science and digital marketing analytics, I don't treat data as stagnant numbers—I view it as an evolving map of operational behavior and customer journeys.

* **🛠 My Tech Stack:** Excel (Advanced Pivots & Analysis), Tableau (Interactive Storytelling), SQL (Window Functions, CTEs, Joins), and Python (Pandas, Seaborn).
* **📬 Connect with Me:** [linkedin](https://www.linkedin.com/in/vaidehibharambeaulagar) | vaidehibh@gmail.com
* **🔗 The Data Pipeline:** This repository focuses strictly on **Exploratory Analysis**. To see how I engineered and audited this raw dataset into a trusted data foundation, check out my [GameZone Data Cleaning Repository](https://github.com/AnalyzeWithVaidehi/gamezone-sales-data-cleaning).

---

## 📌 Project Overview & The SCAN Framework
An operations manager asked an initially vague but critical question: *"How did sales look over the COVID years?"* To translate this ambiguity into a concrete data strategy, I deployed the **SCAN Framework** to analyze over 20,000 clean transactional records spanning 2019 to 2022:

1. **S - Stakeholder Goals:** Identified key personas (Product, Marketing, and Finance managers) and established `USD Price` (Revenue) as our core KPI.
2. **C - Columns & Coverage:** Isolated purchase/shipping timestamps, product descriptions, regional tags, and marketing acquisition metadata.
3. **A - Aggregates & Anomalies:** Determined high-level baseline metrics (~$6.1M in cumulative revenue, with massive monthly swings shifting from $80K to $500K).
4. **N - Notable Segments:** Sliced data across deep operational dimensions (Regions, Marketing Channels, and Products) to find the exact drivers of growth and contraction.

---

## 🧠 High-Level Findings: Slicing the Dimensions
Initial exploratory analysis across the dimensions revealed clear operational baseline behaviors:

* **💰 Top-Line Capture:** Total revenue across the lifecycle reached approximately **$6.1 Million USD**.
* **📦 Product Champions vs Laggards:** The **27in 4K Gaming Monitor** emerged as the ultimate rainmaker, generating nearly **$2 Million** in individual sales. Conversely, the gaming headset sat at the bottom (~$800K), indicating potential underperformance or inventory allocation issues.
* **📣 Channel Dominance:** **Direct Traffic** acts as the primary engine driving customer acquisition. All other promotional channels lag behind significantly, exposing an over-reliance on organic discovery.

---

## 🔍 Executive Deep Dives: Finding the "Why"
By moving past high-level aggregates and combining dimensions, I uncovered critical, systemic anomalies that demand executive intervention:

### 1. The Global 2020 Macro-Spike 📈
The data clearly maps the pandemic-era surge in global gaming demand. Revenue more than doubled in early 2020, reaching historic all-time highs in September and December of 2020. This was followed by a sharp global correction across *all* regions in early 2021, proving a macroeconomic shift rather than a localized drop in performance.

### 2. The Post-Holiday Crash & The PS5 Regional Anomaly 📉
While top products like the Gaming Monitor and Nintendo Switch maintained predictable seasonal rhythms globally, the **Sony PlayStation 5 Bundle** exhibited highly alarming regional behavior. 

At the end of December 2020, revenue experienced a catastrophic crash, plonking from **~$72K down to $30K**. By isolating variables, I pinpointed the cause:
* **The Root Cause:** This crash was heavily concentrated in the **North America (NA) and EMEA** markets.
* **The Mechanics:** It was driven by a twin failure—a sharp drop in **Order Count** (fewer checkouts) running alongside a simultaneous plunge in **Average Order Value (AOV)** specifically for the PlayStation 5 line. Because the PS5 bundle commands the highest unit price in our catalog, a dip in its volume disproportionately harmed the company's bottom line.

---

## 🚀 Data-Driven Recommendations for each Team

* **For the Finance & Supply Chain Teams:** The Gaming Monitor, Nintendo Switch, and PS5 bundle anchor our financial health. Supply chain configurations must protect inventory levels on these three specific products to avoid severe stockout hazards during high-velocity Q4 holiday windows.
* **For the Marketing Team:** Intervene immediately to address our over-reliance on Direct Traffic. Investigate why our affiliate and email funnels are failing to scale, and study the exact promotional mix used during the December 2020 super-cycle to reverse the NA/EMEA transaction drop.
* **For the Product Team:** Conduct a targeted review of the PS5 performance in NA/EMEA. We need to verify if this post-holiday crash was caused by localized stock shortfalls, an unannounced pricing play by a major competitor, or a disruptive checkout UI bug on our web/mobile platform.

---

## 🖥 Interactive Visualizations
The complete interactive visual data story for this project is hosted live. 
* **Explore the Dashboard:** [Vaidehi's GameZone EDA Tableau Workbook](https://public.tableau.com/app/profile/vaidehi.bharambe/viz/GameZoneEDAAnalysis/overallUSD)

---

## 📂 What’s Inside This Repository?
* `gamezone-orders-data-cleaned.xlsx`: My clean dataset from my [GameZone Data Cleaning Repository](https://github.com/AnalyzeWithVaidehi/gamezone-sales-data-cleaning)
* `insights_logs.xlsx`: My clean audit ledger tracking initial aggregates, outlier metrics, dimensional segments, and final strategic plays.
* `issues_logs.xlsx`: The fundamental multidimensional matrices calculating monthly, regional, and product revenue structures.
* `My thought Process.pdf`: My live analytical journal capturing every hypothesis, step-by-step framework application, and raw deduction made during the sprint.

---
*💡 What's next? Now that the data is clean and the foundational insights are completely mapped, my final phase is transitioning these static discoveries into an interactive executive dashboard layout in Power BI!*
