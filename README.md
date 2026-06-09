# ENVS-193DS_spring-2026_final
Final Assignment for ENV S 193DS

# General Information

**Author:** Will Grimsich  
**Course:** ENVS-193DS, Spring 2026  
**Affiliation:** UC Santa Barbara  
**Date:** June 9, 2026

This repository contains the final assignment for ENVS-193DS (Environmental Studies Data Science). The project addresses three problems: (1) identifying and improving gaps in statistical communication in a research report on American Avocet (*Recurvirostra americana*) microhabitat use, (2) a binomial logistic regression analysis examining how acacia ant species and tree height influence bird nest occurrence in whistling thorn trees (*Vachellia drepanolobium*) using data from Lujan et al. (2023), and (3) an affective/exploratory visualization and Kruskal-Wallis analysis of personal screen time and exercise data.

---

# Data and File Overview

```
ENVS-193DS_spring-2026_final/
├── README.md
├── code/
│   └── Final.qmd               # Main Quarto document containing all analysis and write-ups
└── data/
    ├── nest_data_final.csv      # Nest box occupancy data from Lujan et al. (2023)
    ├── exercise.csv             # Raw personal exercise and screen time data
    ├── exercise_clean.csv       # Cleaned version of personal exercise and screen time data
    └── metadata                 # Metadata file describing variables in nest_data_final.csv
```

## Data Descriptions

**nest_data_final.csv**  
Nest box occupancy data from: Lujan, E., Nielsen, R., Short, Z., Wicks, S., Nderitu Watetu, W., Malingati Khasoha, L., Palmer, T. M., Goheen, J. R., & Alston, J. M. (2023). Data, code, and metadata for: Symbiotic acacia ants drive nesting behavior by birds in an African savanna [Data set]. Zenodo. https://doi.org/10.5281/zenodo.8373322  
Key variables include `case_control` (binary: 1 = nest present, 0 = nest absent), `ant_species` (acacia ant species code), and `height_cm` (tree height in centimeters).

**exercise.csv**  
Raw personal data collected daily by Will Grimsich during Spring 2026. Contains records of daily screen time (minutes), exercise time (minutes), and exercise type (Gym, Run, No Exercise, Gym + Run).

**exercise_clean.csv**  
Cleaned version of exercise.csv with standardized column names (snake_case). Contains the same variables as exercise.csv after processing with `janitor::clean_names()`.

**metadata**  
Describes the variables, units, and coding conventions for nest_data_final.csv, as provided by Lujan et al. (2023).

---
# Rendered Output

[Output](https://github.com/wgrimsich/ENVS-193DS_spring-2026_final/blob/main/code/Final.pdf)