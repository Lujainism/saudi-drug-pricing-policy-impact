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
notebooks/
├── 01_web_scraping.ipynb
├── 02_data_cleaning.ipynb
├── 03_data_linkage.ipynb
├── 04_econometric_analysis.ipynb
└── 05_visualization_results.ipynb
scripts/
└── helper_functions.py
requirements.txt



## Author
**Lujain Alassaf**  
Master of Science in Health Policy — Stanford University (2025)  
