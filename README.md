# saudi-drug-pricing-policy-impact
Code and workflow for my Stanford MS thesis analyzing Saudi Arabia’s 2021 drug pricing policy using econometric (DiD) models. 

## Data
Raw data were obtained from **GlobalData**, which requires licensed access and cannot be shared publicly.  
The repository includes the full analytical pipeline but not the source data.


## Overview
- Data integration and cleaning across FDA, EMA, MHRA, and SFDA approval datasets  
- Web scraping scripts (structure only; no proprietary endpoints)  
- Econometric modeling (OLS, DiD with fixed effects)  
- Visualization of launch delays by therapeutic area and cost tier


## Tools
Python (pandas, NumPy, statsmodels, scikit-learn, BeautifulSoup, requests, fuzzywuzzy, matplotlib, seaborn)

## Repository Structure

- [01_web_scraping.ipynb](https://github.com/Lujainism/saudi-drug-pricing-policy-impact/blob/main/01_web_scraping.ipynb) — Demonstrates the workflow used to retrieve missing SFDA registration year data from public sources. No proprietary data included.
- [02_data_cleaning_linkage.ipynb](https://github.com/Lujainism/saudi-drug-pricing-policy-impact/blob/main/02_data_cleaning_linkage.ipynb) — Performs data cleaning, standardization, and record linkage across EMA, FDA, MHRA, and SFDA approval datasets using deterministic and fuzzy-matching methods. Before this step, the SFDA dataset—retrieved from GlobalData—was matched with the web-scraped SFDA data using National Drug ID to populate the missing registration year field prior to integration.
- [03_main_analysis.ipynb](https://github.com/Lujainism/saudi-drug-pricing-policy-impact/blob/main/03_main_analysis.ipynb) — Performs the main analysis, including data manipulation, computation of key analytical variables, and model preparation. This notebook conducts exploratory data analysis, builds the primary econometric models (Difference-in-Differences with year fixed effects and full control variables). It also generates descriptive and regression summary tables, automatically formatted and styled for publication—ready to be exported or directly included in reports and manuscripts.

### Supporting Documentation
- [linkage_methodology.pdf]([link_to_file](https://github.com/Lujainism/saudi-drug-pricing-policy-impact/blob/main/linkage_methodol.pdf) — Details the linkage process across EMA, FDA, MHRA, and SFDA datasets, including standardized ID, fuzzy matching, and manual verification.
- [sensitivity_checks.pdf]([link_to_file](https://github.com/Lujainism/saudi-drug-pricing-policy-impact/blob/main/senstivity_checks.pdf) — Describes the linkage quality assessments and model robustness checks, consistent with Appendices B–C of the thesis.


## Author
**Lujain Alassaf**  
Master of Science in Health Policy — Stanford University (2025)  
