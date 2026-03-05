# Executive A/B Experiment Analysis: Landing Page Conversion Test

This project demonstrates a full A/B experiment analysis for an e-commerce landing page.

The goal of the experiment was to understand whether a **new landing page** increases the **conversion rate** compared to the **old page**.

The dataset contains id, time, con_treat,	page, converted. 
The analysis was performed in Python using a Jupyter Notebook.

## Project workflow

1. Load and inspect the dataset  
2. Data validation and cleaning  
3. Remove incorrect experiment assignments  
4. Deduplicate users  
5. Calculate conversion metrics  
6. Run statistical tests (Z-test)  
7. Calculate confidence interval  
8. Check experiment validity (SRM test)  
9. Estimate required sample size  

The results of the analysis are collected in JSON and sent to the OpenAI API to generate a **structured executive report**.

## Tools used

- Python  
- Pandas  
- Statsmodels  
- OpenAI API  
- Pandoc (Markdown → PDF)

## Output

The final deliverable is an **executive business report** that explains:

- experiment results  
- statistical significance  
- potential business impact  
- recommendation for decision makers
