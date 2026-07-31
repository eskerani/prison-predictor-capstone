# Backlog: Crime and What Else? Investigating the Predictive Power of Social Factors on Incarceration Rates

This file is the **human-readable mirror** of the [GitHub Projects (v2) Iterative Development board](https://docs.github.com/en/issues/planning-and-tracking-with-projects/learning-about-projects/about-projects) for this repo. Every row here is also a GitHub issue, added to the board, tagged with a milestone label, and sized.

## Conventions

- Each item has: id, title, hypothesis or user story, **Create / Observe / Analyze** triple, milestone tag, size.
- Items are ordered top to bottom by **priority**.
- Milestone tags: `M1-proposal`, `M2-data-summary`, `M3-poster-draft`, `M4-writeup-draft`, `M5-final`, `infra`, `ethics`.
- Sizes: S, M, L, XL.
- The board has five columns: `Backlog` → `Create` → `Observe` → `Analyze` → `Done`. Each column is the *phase of work happening on a single PBI right now*, not a work type. See the [Iterative Development board explainer](https://courses.lpcordova.phd/data510/project-framework/#github-projects-board-per-project-iterative-development-board) for what each column means and when to advance a card.
- WIP cap: `Create + Observe + Analyze` ≤ `owners + 1` at any time.
- Definition of Ready and Definition of Done live in [`CHARTER.md`](CHARTER.md).

## Items

### PBI-001

- **Title:** Source race data
- **Hypothesis:** Data about race will be the hardest to find!
- **Create:** comment several options for data sets.
- **Observe:** document the scope and variables of each data set.
- **Analyze:** choose a data set that is the best fit.
- **Tag:** `M1-proposal`
- **Size:** M
- **GitHub issue:** [link](https://github.com/eskerani/prison-predictor-capstone/issues/1)

### PBI-002

- **Title:** Finalize research question
- **Hypothesis:** We can state the project's research question in one sentence that names the population, the predictor or treatment, and the outcome.
- **Create:** make any necessary edits to the current research question.
- **Observe:** compare the draft question to the PRIDE framework.
- **Analyze:** finalize changes.
- **Tag:** `M1-proposal`
- **Size:** S
- **GitHub issue:** [link](https://github.com/eskerani/prison-predictor-capstone/issues/2)

### PBI-003

- **Title:** Choose a machine learning method to use
- **Hypothesis:** I will need to find one algorithm that would work best with non-linear, highly variable data (possibly in an ensemble). 
- **Create:** list options for methods to use.
- **Observe:** find pros and cons of each relative to the data I have.
- **Analyze:** choose an algorithm.
- **Tag:** `M1-proposal`
- **Size:** M
- **GitHub issue:** [link](https://github.com/eskerani/prison-predictor-capstone/issues/3)

### PBI-004

- **Title:** Get data sources approved
- **Hypothesis:** I think my data sources will be good but I will find out. 
- **Create:** write a discord message to Professor Cordova.
- **Observe:** look at his answer.
- **Analyze:** NA
- **Tag:** `M1-proposal`
- **Size:** S
- **GitHub issue:** [link](https://github.com/eskerani/prison-predictor-capstone/issues/4)

### PBI-005

- **Title:** Create ERD for data
- **Hypothesis:** I will diagram a reasonable method of data organization. 
- **Create:** make a table for each data source.
- **Observe:** find connections between the tables.
- **Analyze:** note any transformations that will be necessary to make the data make sense
- **Tag:** `M1-proposal`
- **Size:** S
- **GitHub issue:** [link](https://github.com/eskerani/prison-predictor-capstone/issues/5)

### PBI-006

- **Title:** Create data cleaning plan
- **Hypothesis:** having a plan of attack will make it easier to approach cleaning data. 
- **Create:** load all raw data into R.
- **Observe:** note issues, anomalies, and any non-standard columns or steps that will need to be taken.
- **Analyze:** in a Google Doc, write down all actions that will need to be performed for each data set in order for it to be ready to combine.
- **Tag:** `M2-data-summary`
- **Size:** M
- **GitHub issue:** [link](https://github.com/eskerani/prison-predictor-capstone/issues/6)

### PBI-007

- **Title:** Clean data
- **Hypothesis:** I can standardize all of my datasets to fit with each other. 
- **Create:** follow the data cleaning plan to make changes to data as needed.
- **Observe:** make sure everything looks good, combine datasets.
- **Analyze:** pull preliminary metrics, correlation coefficient for all variables.
- **Tag:** `M2-data-summary`
- **Size:** M
- **GitHub issue:** [link](https://github.com/eskerani/prison-predictor-capstone/issues/7)
 
### PBI-008

- **Title:** Write SVR pseudocode
- **Hypothesis:** I can re-use the same code outline to train several different SVR models. 
- **Create:** write repeatable pseudocode.
- **Observe:** test with one variable set.
- **Analyze:** troubleshoot any errors until code is working as planned.
- **Tag:** `M3-draft-poster`
- **Size:** S
- **GitHub issue:** [link](https://github.com/eskerani/prison-predictor-capstone/issues/8)

### PBI-009

- **Title:** Run SVR
- **Hypothesis:** either crime or police spending will be the most accurate.
- **Create:** building off of the pseudocode, write code that will run SVR for all variables.
- **Observe:** compare graphs and metrics for all models.
- **Analyze:** document accuracy and evaluate which variable performed the best.
- **Tag:** `M3-draft-poster`
- **Size:** M
- **GitHub issue:** [link](https://github.com/eskerani/prison-predictor-capstone/issues/9)

### PBI-010

- **Title:** Draft visualizations
- **Hypothesis:** A line graph will likely be the most understandable kind of plot.
- **Create:** draft 3 different visualization methods with pen and paper.
- **Observe:** write down the pros and cons of each visualization style.
- **Analyze:** choose the best method to use as primary visualization for poster.
- **Tag:** `M3-draft-poster`
- **Size:** S
- **GitHub issue:** [link](https://github.com/eskerani/prison-predictor-capstone/issues/10)

### PBI-011 - PBI-015

- **Title:** Clean individual datasets
- **NOTE:** Each of these issues corresponds to one dataset and has been created as a sub-issue under PBI-007. All have the same create/observe/analyze triple. 
- **Hypothesis:** tracking the progress of each dataset individually will make my life easier.
- **Create:** follow the data cleaning plan to make changes to data as needed.
- **Observe:** make sure everything looks good.
- **Analyze:** pull preliminary metrics.
- **Tag:** `M2-data-summary`
- **Size:** S
- **GitHub issue:** [PBI-011](https://github.com/eskerani/prison-predictor-capstone/issues/11) / [PBI-012](https://github.com/eskerani/prison-predictor-capstone/issues/12) / [PBI-013](https://github.com/eskerani/prison-predictor-capstone/issues/13) / [PBI-014](https://github.com/eskerani/prison-predictor-capstone/issues/14) / [PBI-015](https://github.com/eskerani/prison-predictor-capstone/issues/15)
