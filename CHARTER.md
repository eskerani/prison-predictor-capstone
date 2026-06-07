# Studio Charter: Crime and What Else? Investigating the Predictive Power of Social Factors on Incarceration Rates

* **Owner team:** Emery Kerani*
* **Owner Product Lead:** Emery Kerani
* **Peer Stakeholder POs:** Mary Rose Krouse, Shanti Brodnick, & Rohan Srinivas Babu
* **Instructor / Sponsor:** Lucas Cordova (`LucasCordova` on GitHub)
* **GitHub repo:** [link](https://github.com/eskerani/prison-predictor-capstone)
* **GitHub Projects board:** [link](https://github.com/users/eskerani/projects/1)
* **Discord category:** `#Project 12: Emery-*`
* **Studio Session:** 1
* **Studio formed:** 5/25/26
* *Note: since I am a solo team, team working agreements have been ommitted from this document.

## Vision

This project aims to examine the prison-industrial complex and the effectiveness of our current criminal legal system. I come at the project with the goal of moving away from incarceration as a solution, based on the idea that incarceration does not adequately address the root causes of violence or crime.

## Mission

I will use machine learning methods to assess the predictive power of crime rates, poverty rates, and racial diversity relative to incarceration rates across the United States and over time.

## Context

- **Users / affected parties:** The primary beneficiaries of this research are incarcerated folks, their families and communities, and others who are most at risk of incarceration. There are many transformative justice organizations that could potentially use the result to advocate for reforms to the criminal legal system. 
- **Data sources (proposed):** Incarceration rates from the Bureau of Justice Stastistics [site](https://csat.bjs.ojp.gov/advanced-query) | Crime rates from The FBI's Crime Data [Explorer](https://cde.ucr.cjis.gov/LATEST/webapp/#/pages/downloads) | Poverty rates from the [US Census](https://www.census.gov/data/tables/time-series/demo/income-poverty/historical-poverty-people.html) | Race data from IPUMS [CPS](https://cps.ipums.org/cps-action/variables/group) | Police expenditure data from the [US Census](https://data.census.gov/table/GOVSSTATEFINTIMESERIES.GS00STATEFIN03?q=State%20and%20Local%20Government%20Finances&nkd=AGG_DESC~SF0158%3ASF0342%3ASF0343%3ASF0344%3ASF0345%3ASF0346%3ASF0365&colSort=AGG_DESC_LABEL~desc)
- **Constraints:** One major constraint is that I cannot possibly interrogate every social factor that may contribute to incarceration, especially given that many may not have data readily available. Doing this project as just one person may also very well be a constraint on how much I can realistically get done.
- **Ethics risks:** All statements will have to be hedged by the fact that I'm only looking at correlation, not causation. There may also be covariance present in the data.

## Success criteria by milestone

- **M1, proposal (W4):** All data sources have been identified, the research question is finalized, and a plan to clean the data is in place.
- **M2, data summary (W7):** All data sources are cleaned and joined, with initial exploratory graphs and descriptive statistics created. 
- **M3, poster rough draft (W10):** Create an initial layout and identify types of visualizations that will work best with the data.
- **M4, write-up rough draft (W12):** Interactive markdown has been drafted; answer to research question as well as background/constraints/etc. have been considered and written.
- **M5, final write-up and poster (W14):** Everything is ready to be presented and accessible to a wide variety of audiences!

## Working agreements (triad with peer POs)

- **Studio Brief due:** by 12pm the Sunday before class, committed to `studio/briefs/W<NN>-<peer>.md` and linked in `#Project 12: Emery-studio` on Discord.
- **Studio Critique due:** by 12pm the Tuesday after class, committed to `studio/critiques/W<NN>-<peer>.md` and linked in `#Project 12: Emery-studio` on Discord.
- **Priority conflict resolution:** owner team integrates briefs in good faith; the instructor arbitrates (as Process Expert) if peer POs and owner team disagree.

## Response SLAs (Service Level Agreements)

A **Service Level Agreement** is a written promise the triad makes about *how fast* each side responds when a specific signal arrives. Every row must have an answer before this Charter is committed. See [Response SLAs](https://courses.lpcordova.phd/data510/project-framework/charter-inception.html#response-slas-service-level-agreements) for the full definition.

| When this signal arrives... | Who responds | By when |
|-----------------------------|--------------|---------|
| Peer PO files a **Studio Brief** (commits to `studio/briefs/...`, links in `#Project 12: Emery-studio`) | Owner team | Acknowledge or react in `#<project>-studio` within 24 hours, with a first-pass adopt / defer / decline call for each item |
| Peer PO files a **Studio Critique** | Owner team | Respond in `#Project 12: Emery-studio` within 24 hours and capture follow-up items into the backlog |
| Owner team posts an **Iteration Review** in `README.md` | Both peer POs | Read before filing the next Brief (on Sunday) and Critique (on Tuesday) |
| Owner team flags a **blocker** in `#Project 12: Emery-blockers` | Instructor, plus any tagged peer PO | Responds by the next Studio Session at the latest; faster if online |
| Anyone asks a clarifying question in `#Project 12: Emery-general` | Whoever is tagged (default: owner team) | Reply within 48 hours, even if the reply is "we will look at this next iteration" |

## Definition of Ready (PBI)

A PBI is ready to be pulled out of `Backlog` and moved into `Create` when it has:

- A one-sentence hypothesis or user story.
- A named **Create**, **Observe**, **Analyze** triple.
- A milestone tag (`M1-proposal`, `M2-data-summary`, `M3-poster-draft`, `M4-writeup-draft`, `M5-final`, `infra`, `ethics`).
- A T-shirt size estimate (S, M, L, XL).
- WIP slack on the board: `Create + Observe + Analyze` is below the team's WIP cap (owners + 1).

## Definition of Done (PBI)

A PBI is done, and may be moved from `Analyze` into `Done`, when:

- The Create artifact is in the repo or linked from the issue.
- The Observe results are recorded somewhere referenceable (notebook output, processed dataset, draft results section).
- The Analyze writeup names a next step (continue, pivot, kill, or decompose into new PBIs).
- A peer PO has either signed off in `#Project 12: Emery-studio` or filed a Studio Critique covering it.
- The card is linked under *Completed PBIs* in the next Iteration Review in `README.md`.

## Context map

> Optional. Replace this block with a Mermaid `flowchart LR` showing how users, data, constraints, and ethics risks flow into the owner team and out to the capstone outcome. See the [`charter-inception.qmd` template](https://courses.lpcordova.phd/data510/project-framework/charter-inception.html) for a starting Mermaid diagram.

## Stakeholder alignment memo (one-page summary)

### Why we exist
This project aims to examine the prison-industrial complex and the effectiveness of our current criminal legal system from an abolitionist perspective. I will use machine learning methods to assess the predictive power of crime rates, poverty rates, and racial diversity relative to incarceration rates across the United States and over time.

### What we will deliver to peer POs every week
- An Iteration Review in this `README.md` by Friday / 8pm
- A summary of which Studio Brief items we adopted, deferred, or declined and why

### What we need from peer POs every week
- A Studio Brief by the end of Sunday for next class (next iteration's requirements, questions, risks)
- A Studio Critique by end of Tuesday for next class (assessment of last week's delivery)

### How to reach us
- Discord category: `#Project 12: Emery-general` (day-to-day), `#Project 12: Emery-studio` (Briefs and Critiques), `#Project 12: Emery-blockers` (impediments)
- GitHub repo: [link](https://github.com/eskerani/prison-predictor-capstone)
- GitHub Projects board: [link](https://github.com/users/eskerani/projects/1)
