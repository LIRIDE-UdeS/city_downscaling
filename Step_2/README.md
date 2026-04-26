# Step 2: Household environmental impact allocation based on socio-economic and demographic factors.

Household environmental impacts estimated in Step 1 are allocated across socioeconomic and demographic (SED) subfactors using expenditure-based shares and concordance tables linking IO sectors to expenditure categories.

## Inputs required 

1. A CSV file containing the environmental impacts at the IO sector level for the studied region and year (generated in Step 1)
2. A concordance file extending the IO sector mapping from Step 1 to link each IO sector to its corresponding expenditure category and allocation proportion, for each SED factor and study year. This file must be prepared by the user. The file 2021_income_corr.xlsx was built for the Province of Quebec, year 2021 and income across five quintiles.
3. A file containing the household-weighted expenditure shares by SED subfactor for each expenditure category. This file must be prepared by the user. The file spending_by_income.xlsx was built using data from Institut de la Statistique du Québec (ISQ).

## Outputs

This step generates two output folders:

1. {IMPACT}_by_category/ — one Excel file per consumption category containing the environmental impacts by SED subfactor. Used as input for Step 3.
2. {IMPACT}_by_subfactor/ — one Excel file per SED subfactor containing the environmental impacts by consumption category. Used as input for Step 4.
