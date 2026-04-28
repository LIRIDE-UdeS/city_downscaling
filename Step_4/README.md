# Step 4: City-level downscaling using identified SED drivers as allocation parameters

City-level environmental impacts are estimated by applying the category-specific SED drivers identified in Step 3 as allocation keys. 

## Inputs required

1. The Excel files generated in Step 2, one per SED factor, containing the environmental impacts per household by consumption category and SED subfactor: `{YEAR}_{IMPACT}_{FACTOR}.xlsx`, located in the `Step_2/` folder.
2. One Excel file per city containing the number of households by SED subfactor, located in the folder specified by `REGION_FOLDER`. Each file must be named `{YEAR}_{city}.xlsx` and include the following columns: `Factor`, `Subfactor`, `Households`. For the Province of Quebec case study, these files were built using data from the 2021 Canadian Census (Statistics Canada).

## Outputs

This step generates the following outputs:

1. `city_results/{YEAR}_{IMPACT}_{city}.xlsx` — one Excel file per city, containing the total emissions, emissions per household, and emissions per capita by consumption category and selected driver.
2. `city_results/{YEAR}_{IMPACT}_cities.pdf` — stacked bar chart comparing city-level emissions across consumption categories, per household and per capita.
3. `{YEAR}_{IMPACT}_cities.png` — same figure saved as a high-resolution PNG (600 dpi).
