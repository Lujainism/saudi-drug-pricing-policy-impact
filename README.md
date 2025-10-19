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
- [02_data_cleaning_linkage.ipynb]([https://github.com/Lujainism/saudi-drug-pricing-policy-impact/blob/main/01_web_scraping.ipynb](https://github.com/Lujainism/saudi-drug-pricing-policy-impact/blob/main/02_data_cleaning_linkage.ipynb) — Performs data cleaning, standardization, and record linkage across EMA, FDA, MHRA, and SFDA approval datasets using deterministic and fuzzy-matching methods. Before this step, the SFDA dataset—retrieved from GlobalData—was matched with the web-scraped SFDA data using National Drug ID to populate the missing registration year field prior to integration.



## Author
**Lujain Alassaf**  
Master of Science in Health Policy — Stanford University (2025)  
