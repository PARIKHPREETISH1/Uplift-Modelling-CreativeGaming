# Uplift Modeling for Targeted Advertising  
Creative Gaming Case Study

## Project Overview
This project applies **uplift modeling** to evaluate the true causal impact of digital advertising for Creative Gaming.  
The goal is to identify which users should be targeted with ads to maximize incremental conversions while minimizing wasted marketing spend.

Unlike traditional response prediction models, uplift modeling measures **incremental lift** by comparing treated and control groups, enabling data driven and causally sound marketing decisions.

---

## Business Problem
Creative Gaming invests heavily in paid advertising campaigns. However, not all users respond positively to ads.

Key challenges include:
• Some users convert organically without ads  
• Some users are negatively impacted by ads  
• Traditional models overestimate campaign effectiveness  

The core business question is:
Which users should receive ads to maximize incremental impact and return on investment?

---

## Project Objectives
• Measure the true causal impact of advertising  
• Identify users who are persuadable through ads  
• Avoid targeting users who do not benefit from ads  
• Improve marketing efficiency and customer experience  

---

## Data Description
The analysis uses experimental data with explicit treatment and control groups.

Datasets included:
• cg_ad_treatment.parquet  
  Users exposed to advertising  

• cg_ad_random.parquet  
  Randomized ad exposure group  

• cg_organic_control.parquet  
  Users not exposed to advertising  

Each dataset contains user level behavioral and engagement features along with conversion outcomes.  
Detailed data dictionaries are provided in markdown files inside the data folder.

---

## Methodology
1. Exploratory Data Analysis  
   Comparison of engagement and conversion behavior across treatment and control groups  

2. Uplift Modeling  
   Estimation of incremental lift by separating treatment effects from organic behavior  

3. Customer Segmentation  
   Classification of users into uplift based segments:
   • Persuadables  
   • Sure Things  
   • Lost Causes  
   • Do Not Disturb  

4. Model Evaluation  
   Use of uplift curves and incremental gain analysis to assess performance

---

## Key Insights
• A distinct segment of users shows strong positive uplift from advertising  
• A significant portion of users converts without ad exposure  
• A small group experiences negative uplift, indicating ad fatigue  
• Targeted advertising based on uplift significantly outperforms random targeting  

---

## Business Impact
• Improved marketing ROI through precise targeting  
• Reduced wasted ad spend  
• Better customer experience by avoiding unnecessary ads  
• Strong foundation for causal marketing decision making  

---

## Tools and Technologies
• Python  
• Pandas and NumPy  
• Scikit learn  
• Jupyter Notebook  
• Parquet data format  

---


---

## Skills Demonstrated
• Causal inference  
• Uplift modeling  
• Marketing analytics  
• Experiment design and evaluation  
• Data driven decision making  
• Business insight generation  

---

## Author
Preetish Parikh  
Master’s in Business Analytics  
University of California, San Diego  

---

## Future Work
• Implement advanced uplift modeling techniques  
• Deploy uplift driven targeting strategy  
• Integrate results into real time campaign optimization
