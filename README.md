# Hurricane Ian (2022) Analysis Study

**Zach Simms**

## Project Overview

This project is a two-part analysis (three-part with additional plots in Milestone 3) of Hurricane Ian (2022), focusing on both observed impacts and model-based forecasts. The goal is to assess the storm’s intensity and evolution as it made landfall in Florida, using multiple datasets and visualizations.

### Objectives
- Analyze the surface impacts of Hurricane Ian, including:
  - Rainfall accumulation
  - Minimum sea-level pressure (MSLP)
  - Maximum wind gusts
  - Storm surge impacts
- Compare observed storm tracks with forecast guidance from the GFS and GEFS models to evaluate model performances.
- Produce advanced visualization of forecast data

## Milestone Summaries

### Milestone 1: Observed Surface Impacts
- **Datasets Used**:
  - [Rainfall and surface observations](https://www.nhc.noaa.gov/data/tcr/AL092022_Ian.pdf) from National Hurricane Center (NHC).
- **Methods**:
  - Processed CSV data using `pandas`.
  - Created visualizations with `matplotlib` and `cartopy`.
- **Accomplishments**:
  - Graphed observed rainfall totals, storm surge, and wind gusts across Florida.
  - Visualized the evolution of MSLP as the storm progressed inland.

### Milestone 2: Forecast vs Observed Track Comparison
- **Datasets Used**:
  - [NOAA Best Track Data](https://noaa.hub.arcgis.com/datasets/20d971f4472e4037af0f260f6454e7ab/about?layer=1) (`ianpreliminarytrack.csv`).
  - GFS and GEFS forecast data via the `Herbie` Python package.
- **Methods**:
  - Extracted GFS and GEFS GRIB2 files and processed them using `xarray`.
  - Adjusted coordinate systems to match observed data.
  - Subset forecast data spatially over Florida.
- **Accomplishments**:
  - Saved forecast fields as CSVs.
  - Compared GFS track of Hurricane Ian (latitude and longitudes) to the observed track.
  - Compared GFS intensity track of Hurricane Ian to the observed intensity.
  - Visualized GFS wind and pressure fields surrounding Hurricane Ian at landfall to the observed intensity.
  - Compared GFS and GEFS predicted sea-level pressure with observed values, as well as the storm's center.
 
### Milestone 3: Advanced Visualization of Forecast Data
- **Objectives**:
  - Explore the ensemble spread and relationships in GEFS forecasts using scatterplots (visualize as spaghetti plots).
  - Visualize GFS model rainfall forecast spatially.
  - Map 10-meter wind speed and direction from the GFS model.
- **Datasets & Tools**:
  - GEFS and GFS model forecast data, accessed via the Herbie Python package.
  - Data processing and visualization with `pandas`, `numpy`, `matplotlib`, and `cartopy`.
- **Methods & Accomplishments**:
  - Produced spaghetti plots to assess relationships and spread among ensemble members for Ian's track location.
  - Created spatial map of GFS-predicted rainfall over Florida during Ian’s landfall.
  - Mapped 10-meter wind speed and direction from the GFS model.

## Tools & Technologies
- Python (pandas, numpy, xarray, matplotlib, cartopy, datetime)
- CSV files
- Herbie (for downloading and processing GRIB2 model data)
- Jupyter Notebooks

## License

[MIT](https://choosealicense.com/licenses/mit/)
