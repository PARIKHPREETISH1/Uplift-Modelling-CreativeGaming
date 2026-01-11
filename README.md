# Uplift Modeling for Targeted Advertising  
## Creative Gaming Case Study

## Overview
This project focuses on applying **uplift modeling** to evaluate and optimize targeted advertising strategies for **Creative Gaming**, a digital gaming company.  
The objective is to identify which customers are **most likely to respond positively to ads** and which customers should **not be targeted**, enabling smarter marketing spend and improved customer experience.

Unlike traditional response models, uplift modeling directly measures the **incremental impact of treatment (ads)** by comparing treated and control groups.

---

## Business Problem
Creative Gaming runs paid advertising campaigns to increase user engagement and conversions. However:

- Not all users respond positively to ads  
- Some users would convert organically without ads  
- Some users may be negatively impacted by ads  

**Key Question:**  
> Which customers should receive ads to maximize incremental lift and avoid wasted marketing spend?

---

## Objectives
- Measure the **true causal impact** of advertising
- Identify **persuadable users** who respond positively to ads
- Avoid targeting users who would convert anyway or react negatively
- Improve **ROI and efficiency** of marketing campaigns

---

## Data Description
The analysis uses randomized experimental data with clear treatment and control groups.

### Datasets
- `cg_ad_treatment.parquet`  
  Users exposed to advertising (treatment group)

- `cg_ad_random.parquet`  
  Randomized ad exposure group for causal comparison

- `cg_organic_control.parquet`  
  Users not exposed to ads (control group)

Each dataset includes:
- User demographics and behavioral features  
- Engagement and conversion indicators  
- Treatment assignment  

Supporting data descriptions are included as markdown files in the `data/` folder.

---

## Methodology
1. **Exploratory Data Analysis (EDA)**
   - User behavior comparison across treatment and control
   - Conversion and engagement patterns

2. **Uplift Modeling Approach**
   - Separation of treatment and control populations
   - Estimation of incremental lift instead of raw response
   - Identification of customer uplift segments:
     - Persuadables
     - Sure Things
     - Lost Causes
     - Do Not Disturb

3. **Model Evaluation**
   - Uplift curves
   - Incremental gain analysis
   - Comparison against random targeting

---

## Key Insights
- A significant portion of users show **positive incremental uplift** when exposed to ads
- Some users convert organically and **do not require paid ads**
- A small segment experiences **negative uplift**, indicating potential ad fatigue
- Targeting only high uplift users can:
  - Reduce ad spend waste
  - Improve conversion efficiency
  - Enhance customer experience

---

## Business Impact
- Improved **marketing ROI** through smarter targeting
- Reduced unnecessary ad exposure
- Clear framework for **causal decision making**
- Scalable approach for future campaign optimization

---

## Tools & Technologies
- Python  
- Pandas, NumPy  
- Scikit-learn  
- Jupyter Notebook  
- Parquet data format  

---

## Project Structure
