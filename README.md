# Dictionary

## Analysis

- `preliminary.Rmd`: Preliminary analysis such as data visualization and counts per state.
- `analysis.Rmd`: Fitting IPP and RF models and producing intensity and probability estimates.

## `data/`

### `pfas data.csv`: 8,910 observed data points

- `DistanceToAirport`: Distance to the nearest Part 139 certified airport (required firefighting inspection). log(meters).
- `Precipitation`: 30 year average of annual precipitation. mm/year.
- `DistanceToMilitaryBase`: Distance to the nearest military installation. log(meters).
- `DistanceToLandfill`: Distance to the nearest landfill. log(meters).
- `DistanceToChem`: Distance to the nearest chemicals manufacturer, as designated by the North American Industry Classification System (NAICS); Industry Code(s) 325-. log(meters).
- `DistanceToRubber`: Distance to the nearest rubber manufacturer, as designated by NAICS; Industry Code(s) 3262-. log(meters).
- `DistanceToTextile`: Distance to the nearest textile manufacturer, as designated by NAICS; Industry Code(s) 313-, 314-. log(meters).
- `DistanceToFnB`: Distance to the nearest food and beverages manufacturer, as designated by NAICS; Industry Code(s) 311-, 3121-. log(meters).
- `DistanceToFurniture`: Distance to the nearest furniture manufacturer, as designated by NAICS; Industry Code(s) 337-. log(meters).
- `DistanceToLeather`: Distance to the nearest leather manufacturer, as designated by NAICS; Industry Code(s) 316-. log(meters).
- `DistanceToMiscellaneous`: Distance to the nearest miscellaneous manufacturer, as designated by NAICS; Industry Code(s) 339-. log(meters).
- `DistanceToPaper`: Distance to the nearest paper mill, as designated by NAICS; Industry Code(s) 322-. log(meters).
- `PopDen`: (Scaled) population density at 0.1 by 0.1 (Lat/Long) grid to which the observation belongs. Integer between 1 and 255.
- `Median.Earnings.Inflation.Adj.2020`: Median earnings, adjusted at 2020 dollar value, at the ZipCode Tabulation Area(ZCTA) to which the observation belongs. Missing values set to 0. 2020 \$.
- `Concentration`: PFOA + PFOS observation. parts per trillion (ppt).
- `Latitude`, `Longitude`: Latitude and Longitude of observation. WGS 84 CRS.
- `STUSPS`: USPS 2 letter state abbreviation.

### `extrapolation data.csv`: 50,000 randomly generated points

- `DistanceToAirport`: Distance to the nearest Part 139 certified airport (required firefighting inspection). log(meters).
- `Precipitation`: 30 year average of annual precipitation. mm/year.
- `DistanceToMilitaryBase`: Distance to the nearest military installation. log(meters).
- `DistanceToLandfill`: Distance to the nearest landfill. log(meters).
- `DistanceToChem`: Distance to the nearest chemicals manufacturer, as designated by the North American Industry Classification System (NAICS); Industry Code(s) 325-. log(meters).
- `DistanceToRubber`: Distance to the nearest rubber manufacturer, as designated by NAICS; Industry Code(s) 3262-. log(meters).
- `DistanceToTextile`: Distance to the nearest textile manufacturer, as designated by NAICS; Industry Code(s) 313-, 314-. log(meters).
- `DistanceToFnB`: Distance to the nearest food and beverages manufacturer, as designated by NAICS; Industry Code(s) 311-, 3121-. log(meters).
- `DistanceToFurniture`: Distance to the nearest furniture manufacturer, as designated by NAICS; Industry Code(s) 337-. log(meters).
- `DistanceToLeather`: Distance to the nearest leather manufacturer, as designated by NAICS; Industry Code(s) 316-. log(meters).
- `DistanceToMiscellaneous`: Distance to the nearest miscellaneous manufacturer, as designated by NAICS; Industry Code(s) 339-. log(meters).
- `DistanceToPaper`: Distance to the nearest paper mill, as designated by NAICS; Industry Code(s) 322-. log(meters).
- `PopDen`: (Scaled) population density at 0.1 by 0.1 (Lat/Long) grid to which the observation belongs. Integer between 1 and 255.
- `Median.Earnings.Inflation.Adj.2020`: Median earnings, adjusted at 2020 dollar value, at the ZipCode Tabulation Area(ZCTA) to which the observation belongs. Missing values set to 0. 2020 \$.
- `Latitude`, `Longitude`: Latitude and Longitude of observation. WGS 84 CRS.
- `STUSPS`: USPS 2 letter state abbreviation.

## `mapping/`

### `mapping pfas.qgz`: QGIS project file used for analyeses

### `shapefiles`: ESRI Shapefiles used for analyeses

- `CONUS`: Shapefile of the Contiguous United States
- `Unbiased States`: Shapefile of the states designated as unbiased states; (CA, CO, MD, MA, MI, NH, NJ, NC, OH, RI, SC, WV, WI)
- `Boston`: Shapefile of the city of Boston

## `results/`

- `100% RF Predictions.csv`: Predicted probabilities of observing PFAS at each observation and extrapolation point as predicted by a random forest model using 100% of the data.
- `100% Intensity Predictions.csv`: Predicted PFAS intensity at each observation and extrapolation point as predicted by an IPP model using 100% of the data.
- `100% Bias Function.csv`: Bias function (probability of the point being sampled) fitted by the IPP model using 100% of the data.
- `50% RF Predictions.csv`: Predicted probabilities of observing PFAS at each observation and extrapolation point as predicted by a random forest model using 50% of the data.
- `50% Intensity Predictions.csv`: Predicted PFAS intensity at each observation and extrapolation point as predicted by an IPP model using 50% of the data.
- `50% Bias Function.csv`:Bias function (probability of the point being sampled) fitted by the IPP model using 50% of the data.

## `figures/`

`tiff` and `svg` files of figures included in the manuscript
