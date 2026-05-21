# NOAA GEFS Data Access and Ensemble Spread Analysis

This repository demonstrates how to access NOAA Global Ensemble Forecast System (GEFS) forecast files from the public Amazon S3 archive and perform basic ensemble forecast analysis using Python in Google Colab.

The project focuses on three workflow steps:

1. Opening GEFS GRIB2 forecast files from Amazon S3
2. Computing ensemble mean and ensemble spread
3. Examining how ensemble spread grows with forecast lead time

## Project Motivation

Ensemble forecast systems are widely used in operational weather prediction to estimate forecast uncertainty. Instead of relying on a single deterministic forecast, GEFS provides multiple forecast members. The disagreement among these members, often measured by ensemble spread, gives useful information about forecast confidence.

This project was developed as a practical scientific programming workflow for working with operational-style NOAA forecast data in Python.

## Data

- Dataset: NOAA Global Ensemble Forecast System (GEFS)
- Source: Public Amazon S3 archive
- File type: GRIB2
- Variable used in this project: 2 m temperature
- Domain: United States / CONUS region
- Tools: Google Colab, Python, xarray, cfgrib, s3fs, numpy, matplotlib

## Repository Structure

```text
noaa-gefs-data/
├── README.md
├── requirements.txt
├── notebooks/
│   ├── 01.open_gefs_files_colab.ipynb
│   ├── 02.ensemble_mean_spread_analysis.ipynb
│   └── 03.gefs_spread_growth_with_lead_time.ipynb
└── figures/
    ├── gefs_ensemble_mean.png
    ├── gefs_ensemble_spread.png
    └── gefs_spread_growth_leadtime.png
```
## AI Assistance Disclosure

Parts of this project were developed with AI assistance for code organization, README drafting, and workflow refinement. All scientific choices, code execution, debugging, and final review were completed by the author.
