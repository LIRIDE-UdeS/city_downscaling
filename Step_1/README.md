# Step 1: Household environmental impact determination by consumption category.

Household environmental impacts are estimated using a multi-regional input-output (MRIO) model and aggregated into consumption categories.

## Inputs required

To calculate the Household environmental impacts of a region, the following input matrices are required:

1. Leontief inverse (L)
2. Final demand for households (Y and Fy)
3. Environmental extensions matrix (S)
4. Characterization matrix (C)

These matrices must be generated using an MRIO model and placed in a folder named 1_Loading_the_data_files/ prior to running the notebook. For the Province of Quebec (Canada) case study, [OpenIO-Canada](https://github.com/CIRAIG/OpenIO-Canada) was used.

Additionally, a concordance file mapping each IO sector to its corresponding consumption category must be prepared by the user and placed in the working directory. The file Aggregation.xlsx was built for the Province of Quebec based on the North American Product Classification System (NAPCS) and the Classification of Products by Activity (CPA). 

## Outputs
This step generates two outputs files:

1. A CSV file containing the environmental impacts at the IO sector level for the studied region and year. 
2. An Excel file containing the environmental impacts and percentage contribution aggregated by consumption category for the studied region and year. 
