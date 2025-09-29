# Traffic Accident Analysis: Uncovering the Impact of Weather on Driver Inattention

---

## Project Overview & Business Value

* **Problem:** Does **weather condition** affect the primary **contributing factors** of traffic accidents? Specifically, does a change in perceived danger (e.g., snow vs. rain) lead to a change in **driver behavior**?
* **Goal:** To determine the relationship between weather and driver inattention/distraction, providing actionable insights for **public safety campaigns** and **traffic enforcement resource allocation**.
* **Outcome:** The analysis revealed that distracted driving accidents are **higher in rainy conditions than in clear conditions**, and **significantly lower in snowy conditions**.

---

## Technical Methodology & Tools

This project demonstrates proficiency in data wrangling, cleaning, analysis, and visualization using the following stack:

| Category | Tools & Libraries Used | Skills Demonstrated |
| :--- | :--- | :--- |
| **Data Acquisition** | Python, `requests` | API/Web Data Integration |
| **Data Processing** | **Pandas**, **NumPy**, SQL (Optional: Mention if you used SQL for initial filtering) | Data Merging, Feature Engineering, Data Consolidation (`Rain: Heavy` → `Rain`) |
| **Data Analysis** | `scipy` (statistical testing, if any), Group-By Aggregations | Hypothesis Testing, Exploratory Data Analysis (EDA) |
| **Visualization** | **Matplotlib**, **Seaborn** (Optional: Mention Tableau/Power BI if you used it to create a final dashboard) | Data Storytelling, Professional Charting |

### Key Analytical Steps:

1.  **Data Merging:** Combined two distinct datasets (Accident Details and Weather) into a single, cohesive DataFrame using a common unique identifier.
2.  **Feature Engineering (Data Consolidation):** Consolidated over 50 specific weather descriptions (e.g., 'Rain: Heavy', 'Snow: Light') into three clean, categorical bins: **Rainy**, **Snowy**, and **Clear/Cloudy**.
3.  **Target Filtering:** Filtered the final dataset to isolate accidents where the primary `Contributing Factor` was **Driver Inattention/Distraction**, establishing a focused target for the analysis.

---

## Key Findings & Interpretation

The visual analysis of distracted driving accidents across the engineered weather bins yielded compelling, non-obvious results:

1.  **Snow → High Caution:** There were **significantly fewer** distracted driving accidents in snowy conditions compared to rainy or clear conditions. This suggests drivers are highly attuned to the **perceived danger** of snow and adjust their attention/behavior accordingly.
2.  **Rain → Underestimated Risk:** Surprisingly, more distracted driving accidents occurred during **rainy conditions** than in clear conditions. This indicates that drivers may be **underestimating the impact of rain** or not adapting their behavior as much as they do for snow.

> **Actionable Insight:** Public safety campaigns should focus on the **risk of distraction during moderate-risk weather like rain**, as drivers seem to have a false sense of security in these conditions.

---

## How to Replicate the Analysis

### Prerequisites:

* **Python 3.x**
* **Libraries:** `pandas`, `numpy`, `requests`, `matplotlib`, `seaborn`, `scipy`

Install dependencies:
```bash
pip install pandas numpy requests matplotlib seaborn scipy
