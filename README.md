# Cancer Mortality Rates

## Overview

This dataset examines factors that affect cancer mortality rates across U.S. counties. The dataset contains county-level data for a random sample of 537 counties. Data were aggregated from multiple public sources, including the American Community Survey (census.gov), clinicaltrials.gov, and cancer.gov.

The dataset can be used for exploratory data analysis, statistical modeling, and research on the relationships between demographic, socioeconomic, and health-related factors and cancer mortality outcomes.

---

## Data Dictionary

| Variable          | Description                                                                          |
| ----------------- | ------------------------------------------------------------------------------------ |
| `cmRate`          | Number of cancer mortalities per 100,000 people                                      |
| `population`      | Population of the county                                                             |
| `medianIncome`    | Median income of the county                                                          |
| `pctPoverty`      | Percent of the county population living in poverty                                   |
| `avgHouse`        | Average household size (number of residents)                                         |
| `medianAge`       | Median age of county residents                                                       |
| `medianAgeM`      | Median age of male county residents                                                  |
| `medianAgeF`      | Median age of female county residents                                                |
| `pctHS`           | Percent of county residents (ages 25+) with a high school diploma                    |
| `pctBach`         | Percent of county residents (ages 25+) with a bachelor’s degree                      |
| `pctEmployed`     | Percent of county residents (ages 16+) who are employed                              |
| `pctUnemployed`   | Percent of county residents (ages 16+) who are unemployed                            |
| `pctPrivateHC`    | Percent of county residents with private health coverage                             |
| `pctEmployerHC`   | Percent of county residents with employer-provided private health coverage           |
| `pctPublicHC`     | Percent of county residents with government-provided health coverage                 |
| `pctWhite`        | Percent of county residents who identify as White                                    |
| `pctBlack`        | Percent of county residents who identify as Black                                    |
| `pctAsian`        | Percent of county residents who identify as Asian                                    |
| `pctOther`        | Percent of county residents who identify as a race other than White, Black, or Asian |
| `rmRace`          | Race with the relative majority (largest percentage) in the county                   |
| `pctMarried`      | Percent of county residents who are married                                          |
| `pctMarriedHouse` | Percent of households that are married households                                    |
| `birthRate`       | Number of live births relative to the number of women in the county                  |
| `region`          | Geographic region of the county                                                      |
| `state`           | State of the county                                                                  |
| `county`          | Name of the county                                                                   |

---

## File Information

* **File type:** CSV
* **Number of observations:** 537
* **Number of variables:** 26

---

## Suggested Analyses

* Examine correlations between socioeconomic indicators and cancer mortality rates.
* Assess regional and demographic disparities in cancer mortality.
* Develop predictive models to identify key factors influencing cancer mortality.
* Visualize variations in health coverage, poverty, or education levels across regions.

---

## Example Usage (Python)

```python
import pandas as pd

# Load data
df = pd.read_csv("cancer_mortality.csv")

# Preview dataset
print(df.head())

# Explore correlations
print(df[['cmRate', 'medianIncome', 'pctPoverty']].corr())
```

---

## Sources

* American Community Survey ([census.gov](https://www.census.gov))
* [clinicaltrials.gov](https://clinicaltrials.gov)
* [cancer.gov](https://www.cancer.gov)
