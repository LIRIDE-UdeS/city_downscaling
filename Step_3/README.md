# Step 3: Drivers’ analysis and identification. 

This step evaluates candidate socioeconomic and demographic (SED) factors as potential allocation drivers for each consumption category using three criteria. Criterion 1 assesses expenditure differentiation based on confidence-bound overlap across SED subfactors. Criteria 2 and 3 assess impact inequality using the Gini coefficient, at the household and per capita levels respectively. 

## Criterion 1: Expenditure differentiation assessment

### Inputs
1. One Excel file per SED factor and study year, containing the mean expenditure and confidence bounds by subfactor and consumption category. The file must include the following columns: Segment, Category, Mean_alloc, Lower_alloc, Upper_alloc. This file must be consistent with the concordance table used in Step 2. For the Province of Quebec case study, the file 2021_Income.xlsx was built using data from the Institut de la Statistique du Québec (ISQ) and the concordance table 2021_Income_corr.xlsx.

### Outputs
This notebook generates two Excel files per SED factor and study year:

1. {YEAR}_{FACTOR}_Criterion1_summary.xlsx — list of consumption categories for which the SED factor meets Criterion 1.
2. {YEAR}_{FACTOR}_Criterion1_pairs.xlsx — detailed pairwise comparison of subfactors for each consumption category, indicating whether each pair shows a significant difference at the household and per capita levels.

## Criteria 2 and 3: Inequality assessment – Gini coefficient

### Inputs
1. The environmental impact files generated in Step 2, located in the {IMPACT}_by_category/ folder, one file per consumption category.
2. The household share and average household size by SED subfactor, specified directly in the notebook parameters (HOUSEHOLD_SHARE and HOUSEHOLD_SIZE).

### Outputs
This notebook generates two Excel files per SED factor and study year:

1. {YEAR}_{FACTOR}_Criterion2_Gini_household.xlsx — Gini coefficient of environmental impact distribution at the household level for each consumption category.
2. {YEAR}_{FACTOR}_Criterion3_Gini_per_capita.xlsx — Gini coefficient of environmental impact distribution at the per capita level for each consumption category.

