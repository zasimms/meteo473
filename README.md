# Hurricane Ian (2022) Analysis Study

**Zach Simms**

## Project Overview

This project is a two-part analysis of Hurricane Ian (2022), focusing on both observed impacts and model-based forecasts. The goal is to assess the storm’s intensity and evolution as it made landfall in Florida, using multiple datasets and visualizations.

### Objectives
- Analyze the surface impacts of Hurricane Ian, including:
  - Rainfall accumulation
  - Minimum sea-level pressure (MSLP)
  - Maximum wind gusts
  - Storm surge impacts
- Compare observed storm tracks with forecast guidance from the GFS model to evaluate model performance.

## Milestone Summaries

### Milestone 1: Observed Surface Impacts
- **Datasets Used**:
  - Rainfall and surface observations from NWS and NHC.
- **Methods**:
  - Processed CSV data using `pandas`.
  - Created visualizations with `matplotlib` and `cartopy`.
- **Accomplishments**:
  - Mapped observed rainfall totals and wind gusts across Florida.
  - Visualized temporal evolution of MSLP as the storm progressed inland.

### Milestone 2: Forecast vs Observed Track Comparison
- **Datasets Used**:
  - NOAA Best Track Data (`ianpreliminarytrack.csv`)
  - GFS forecast data via the `Herbie` Python package.
- **Methods**:
  - Extracted GFS GRIB2 files and processed them using `xarray`.
  - Adjusted coordinate systems to match observed data.
  - Subset forecast data spatially over Florida.
- **Accomplishments**:
  - Saved forecast fields as CSVs.
  - Compared GFS-predicted sea-level pressure with observed values.

## Tools & Technologies
- Python (pandas, xarray, matplotlib, cartopy)
- Herbie (for downloading and processing GRIB2 model data)
- Jupyter Notebooks

## License

[MIT](https://choosealicense.com/licenses/mit/)
