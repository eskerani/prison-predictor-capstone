# Welcome to the landing page for *Crime and What Else? Investigating the Predictive Power of Social Factors on Incarceration Rates*
(A capstone project completed by Emery Kerani)

This project seeks to explore associations between social factors and national incarceration rates, in order to investigate whether crime or other variables (e.g. racial diversity)
are better predictors of the national incarceration rate across time. 

If you would like to explore the past deliverables for this project, they can be found in the following folders:
* [Milestone 1/Project Proposal](https://github.com/eskerani/prison-predictor-capstone/tree/main/deliverables/M1-proposal)
* [Milestone 2/Data Summary](https://github.com/eskerani/prison-predictor-capstone/tree/main/deliverables/M2-data-summary)
* [Milestone 3/Draft Poster](https://github.com/eskerani/prison-predictor-capstone/tree/main/deliverables/M3-poster-draft)
* [Milestone 4/Draft Writeup](https://github.com/eskerani/prison-predictor-capstone/tree/main/deliverables/M4-writeup-draft)
* [Milestone 5/Final Deliverables](https://github.com/eskerani/prison-predictor-capstone/tree/main/deliverables/M5-final) 

If you would like to investigate the data or cleaning process, navigate to the [data folder](https://github.com/eskerani/prison-predictor-capstone/tree/main/data). 
Raw data is contained in the `raw` folder; preliminary findings/EDA are in the `interim` folder; and the final combined dataset and script used to clean it are in the `processed` folder.

### Visualizations
The visualizations used on the poster are reproduced here, in case you would like a closer look:

<img width="1176" height="1176" alt="capstone data sketch drawio" src="https://github.com/user-attachments/assets/b52e4b0b-382d-4c7d-b6f5-d2ccd428b37c" />

*Figure 1: A diagram of the pipeline used for this project, from ingestion to modeling*

---

<img width="1701" height="1413" alt="all_graph" src="https://github.com/user-attachments/assets/bc0d716a-e3b0-401a-8e9a-6fa06b920ada" />

*Figure 2: A time series graph displaying the national incarceration rate compared to SVR predictions based on police spending data only (green dotted) and all features (orange dashed)*

---

<img width="2009" height="1413" alt="rmse_graph" src="https://github.com/user-attachments/assets/549f62ff-440f-469a-8e09-493aa71ade62" />

*Figure 3: A bar plot depicting the RMSEs of all models for comparison*

---

<img width="2217" height="933" alt="poster_table" src="https://github.com/user-attachments/assets/ec619f99-bb3f-4105-802e-33ff6db5d13d" />

*Table 1: A table displaying the results and stats for all models/variables. The best results are highlighted in darker purple, with worse results in lighter shades*

---

### Full data citations
1. Bureau of Justice Statistics. Corrections Statistical Analysis Tool [dataset]. n.d. https://csat.bjs.ojp.gov/advanced-query
2. Sarah Flood, Miriam King, Renae Rodgers, Steven Ruggles, J. Robert Warren, Daniel Backman, Etienne Breton, Grace Cooper, Julia A. Rivera Drew, Stephanie Richards, David Van Riper, and Kari C.W. Williams. IPUMS CPS: Version 13.0 [dataset]. Minneapolis, MN: IPUMS. 2025. https://doi.org/10.18128/D030.V13.0
3. Federal Bureau of Investigation. Summary Reporting System [dataset]. 2025. https://cde.ucr.cjis.gov/LATEST/webapp/#/pages/downloads
4. United States Census Bureau. Annual Survey of State and Local Government Finances [dataset]. 2026. Published by Nikhita Airi, Lucy Dadayan, Gabriella Garriga, and Kim Rueben at the Urban Institute. https://state-local-finance-data.taxpolicycenter.org/pages.cfm
5. United States Census Bureau. Number of Poor and Poverty Rate by State [dataset]. 2025. https://www.census.gov/data/tables/time-series/demo/income-poverty/historical-poverty-people.html
