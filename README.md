# Remote Work Policies and Employee Productivity Post-COVID

Replication code and figures for the paper:

**"Remote Work Policies and Employee Productivity in the Post-COVID Era:
A Mixed-Methods Analysis Using BLS ATUS and Glassdoor Sentiment Data"**

Author: Pooja Bohara
Institution: York St John University, London Campus

---

## Overview

This repository contains the complete analysis code used in the paper,
implemented in Google Colab (Python 3.12).

The study combines:
- **BLS American Time Use Survey (ATUS)** 2019 and 2023 microdata
- **Glassdoor employee reviews** (via Kaggle)

Using two analytical methods:
- Difference-in-Differences (DiD) regression
- VADER NLP sentiment analysis

---

## Key Results

| Finding | Value |
|---|---|
| DiD coefficient (H1) | +48.87 min, p < 0.001 |
| Knowledge workers (H3) | +55.0 min, p < 0.001 |
| Young workers 18–34 (H5) | +91.1 min, p < 0.001 |
| Senior workers 55–64 (H5) | +7.0 min, p = 0.780 |
| Sentiment decline 2019→2021 | 0.6952 → 0.6692, t = 4.42 |

---

## Repository Structure
```
├── remote_work_productivity_analysis.ipynb   # Full analysis notebook
├── fig1_work_minutes.png                     # Figure 1: Work minutes by group
├── fig2_subgroups.png                        # Figure 2: DiD by subgroup
├── fig3_sentiment.png                        # Figure 3: Glassdoor sentiment
├── fig4_adoption.png                         # Figure 4: Remote work adoption
└── README.md
```

---

## How to Reproduce

### Step 1 — Open in Google Colab
Click the badge below or open
[remote_work_productivity_analysis.ipynb](remote_work_productivity_analysis.ipynb)
directly in Colab.

### Step 2 — Download ATUS data
Download 2019 and 2023 microdata files directly from BLS:
- https://www.bls.gov/tus/datafiles/atusresp-2019.zip
- https://www.bls.gov/tus/datafiles/atusact-2019.zip
- https://www.bls.gov/tus/datafiles/atussum-2019.zip
- https://www.bls.gov/tus/datafiles/atusresp-2023.zip
- https://www.bls.gov/tus/datafiles/atusact-2023.zip
- https://www.bls.gov/tus/datafiles/atussum-2023.zip

Upload the extracted `.dat` files to Google Drive and mount in Colab.

### Step 3 — Download Glassdoor data
Download from Kaggle:
https://www.kaggle.com/datasets/davidgauthier/glassdoor-job-reviews

### Step 4 — Run all cells in order

---

## Dependencies
```
pandas
numpy
scipy
statsmodels
vaderSentiment
matplotlib
```

All installable via pip inside Colab.

---

## Data Sources

- BLS ATUS: https://www.bls.gov/tus/data.htm (public domain)
- Glassdoor Reviews: https://www.kaggle.com/datasets/davidgauthier/glassdoor-job-reviews

---

## License

MIT License — free to use and adapt with attribution.
