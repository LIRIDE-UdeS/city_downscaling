# Step 1: Household environmental impact determination by consumption category.

Household environmental impacts are estimated using a multi-regional input-output (MRIO) model and aggregated into consumption categories.

## Inputs required

To calculate the Household environmental impacts of a region, the following input matrices are required:

1. Leontief inverse (L)
2. Final demand for households (Y and Fy)
3. Environmental extensions matrix (S)
4. Characterization matrix (C)

These matrices must be generated using an MRIO model and placed in a folder named 1_Loading_the_data_files/ prior to running the notebook. For the Province of Quebec (Canada) case study, [OpenIO-Canada](https://github.com/CIRAIG/OpenIO-Canada) was used.

Additionally, the a concordance mapping each IO sector to its corresponding consumption category must be prepared by the user. The file: Aggregation.xlsx it was built for the case study, and it is based on the North American Product Classification System (NAPCS) and the Classification of Products by Activity (CPA). 

## Outputs
This step generates two outputs:
1. The studied environmental impact per IO sector, in the presented study case the file is the climate change short-term emissions of the households for the Province of Quebec 2021, file CC_Households_Quebec_2021.csv — Climate Change impacts (kg CO2 eq) at the IO sector level for the Province of Quebec (2021). Used as input for Step 2.
2. The studied environmental impact per consumption category. In the example is CC_by_consumption_category_2021.xlsx 

