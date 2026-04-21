# CIVE 202 – Project 4: NRI Sensitivity Analysis

**Group M:** Jacob Kosmicki, Jacob Lamoureux, Eli Speth
**Course:** CIVE 202 – Civil Engineering Analysis II
**Instructor:** Dr. Lane
**Date:** April 2026

---

## Project Overview

This project evaluates potential bias in the FEMA National Risk Index (NRI) by comparing results from Florida and Alaska—two states with very different hazard profiles.

The standard NRI formulation is:

```
Risk Index = Expected Annual Loss × Social Vulnerability / Community Resilience
```

We compare this with a custom weighted model that incorporates normalized variables and an interaction term to emphasize areas with both high loss potential and high social vulnerability.

---

## Repository Contents

| File                              | Description                                                                         |
| --------------------------------- | ----------------------------------------------------------------------------------- |
| `GroupM_Project4_Final.ipynb`     | Main Jupyter Notebook with all data loading, cleaning, analysis, and visualizations |
| `GroupM_AnnotatedCode.docx`       | Line-by-line annotated explanation of the notebook code                             |
| `GroupM_Project4_Report.docx`     | Written report summarizing findings, methodology, and ethical analysis              |
| `Project-4_SOW_GroupM.docx`       | Scope of Work document                                                              |
| `GroupM_Project4_GanttChart.xlsx` | Gantt chart of project activities                                                   |
| `GroupM_Timesheet`                | Timesheet with billing information                                                  |
| `All_Data_File.zip`               | All raw and cleaned data files (see Data Setup below)                               |
| `README.md`                       | This file                                                                           |

---

## Data Setup

All data files are bundled in `All_Data_File.zip`. **You must download and extract this file before running the notebook.**

1. Download `All_Data_File.zip` from this repository
2. Extract the contents into the **same folder** as `GroupM_Project4_Final.ipynb`
3. Your folder should contain:

```
NRI_Table_CensusTracts_Florida.csv
NRI_Table_CensusTracts_Alaska.csv
Florida.csv
Alaska.csv
NRIDataDictionary.csv
NRI_HazardInfo.csv
```

### Shapefiles

The shapefiles were too large for github so they are accessible through a OneDrive link:
https://1drv.ms/f/c/c49b30d93d0cb452/IgCRA_4WqOldQ6t60Px7XrLSAUMMAHcYx2c7rxdfJ4Jwrew?e=wVkm2S

Download and place them in the same working directory (or update paths in the notebook if stored elsewhere).

---

## How to Run the Notebook

1. Install required libraries:

   ```
   pip install pandas numpy matplotlib seaborn geopandas
   ```

2. Open `GroupM_Project4_Final.ipynb` in Jupyter Notebook or JupyterLab

3. Run all cells (`Kernel → Restart & Run All`)

---

## Data Sources

* FEMA National Risk Index (NRI):
  https://hazards.fema.gov/nri/data-resources

* CDC/ATSDR Social Vulnerability Index (SVI):
  https://www.atsdr.cdc.gov/place-health/php/svi/svi-data-documentation-download.html

* NRI Scores and Ratings Documentation:
  https://hazards.fema.gov/nri/understanding-scores-ratings
