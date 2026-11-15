# County Rainfall and Planting Advisory

## Project summary
This project analyses monthly rainfall readings for Nairobi, Nakuru, Kisumu, Mombasa, and Machakos. It cleans the manually entered Machakos data, uses NumPy to calculate rainfall patterns, and exports a five-county summary to `rainfall_summary.csv`.

## How to run the notebook
1. Clone or download this repository and open a terminal in the project folder.
2. Install dependencies using `python -m pip install -r requirements.txt`.
3. Start Jupyter with `jupyter notebook`, open `rainfall_analysis.ipynb`, then choose **Kernel → Restart & Run All**.

## Planting advisory
- Nairobi, Nakuru, Kisumu, and Mombasa have their highest consecutive two-month rainfall totals in **April–May** in this dataset.
- Machakos has its highest consecutive two-month rainfall total in **November–December**, after imputation of its invalid readings.
- Treat these windows as historical rainfall guidance, not a guarantee; farmers should also consider crop type, soil conditions, drainage, and current weather forecasts.

## Data quality caveat
Machakos contained `N/A` for April and an empty value for September. Both were imputed with **68 mm**, the rounded mean of its ten valid monthly readings. This estimation may affect Machakos's annual total and planting window. The supplied data represents one set of monthly readings and is not a long-term climate normal.
