# Reproduction instructions

This document details how to reproduce this project. Follow the steps below:

1. Navigate to the main page of this repository.
2. Hit the green "code" button and copy the URL that pops up under "Clone".
3. Open your terminal or CLI.
4. Enter the command `git clone url`, with the url replaced by what you copied. This creates a local clone of the repository.
5. The copied repository should now show up under your GitHub profile.
6. Make sure you have all packages noted in `requirements.txt` (in the repository's main page) downloaded for both R and Python.

**Cleaning:**

7. Follow the instructions in `data/README.md` to download each dataset or use the versions already present in the `data/raw` folder (**note**: you will still need to follow the instructions to acquire IPUMS data).
8. Making sure that all datasets are in the same folder as the cleaning script, run `data/processed/data_cleaning.qmd`.
9. This should create two files: `all_data_combined.csv` and `all_data_processed.csv`.
10. Move `all_data_combined.csv` into the `deliverables/M5-final` folder.

**Analysis:**

11. Open `deliverables/M5-final`.
12. Run `analysis.qmd` to generate results and plots.
13. Render `writeup_v2.qmd` to generate the final writeup. 
