
<!-- README.md is generated from README.Rmd. Please edit that file -->

# Berkshire Hathaway Energy Project

## By: Brian Nielsen, Jack Saele, Larry Rabang, Gabe D’Alessio, and Saul Varshavsky

## Acknowledgements:

We give credit to Drew Covington, Theresa Sheridan, and Jack Schwartz
for providing us some code that we ended up using to help answer the business
problem. Additionally, we give credit to Landon Norkus for providing us the weather data.

## Sources:

https://stackoverflow.com/questions/42996544/how-to-remove-the-date-from-a-column-containing-both-date-and-time-using-r
https://stackoverflow.com/questions/15917824/checking-for-identical-columns-in-a-data-frame-in-r
https://statisticsglobe.com/r-write-read-multiple-csv-files-for-loop 
https://www.statology.org/r-drop-column/
https://youtu.be/S7MkI6M4suc
https://www.rdocumentation.org/packages/Rcmdr/versions/2.0-4/topics/stepwise

https://www.statology.org/inner-join-in-r/#:~:text=We%20can%20use%20the%20merge%20%28%29%20function%20in,5%20G%2020%2010%206%20H%2028%208 

https://www.statology.org/inner-join-in-r/#:~:text=We%20can%20use%20the%20merge%20%28%29%20function%20in,5%20G%2020%2010%206%20H%2028%208 
https://www.maths.usyd.edu.au/u/UG/SM/STAT3022/r/current/Misc/data-visualization-2.1.pdf
https://r-graph-gallery.com/
https://stackoverflow.com/questions/20220424/ggplot2-bar-plot-no-space-between-bottom-of-geom-and-x-axis-keep-space-above






<!-- badges: start -->
<!-- badges: end -->

### Business Problem

Our project aims to solve the following business problem: Which turbine
sensor readings and environmental conditions are more likely to result
in the occurrence of a fault code within 24 hours from the dates and times at
which the turbine sensor readings and environmental conditions were recorded?

### R Code Used

Our team went through a lot of trial and error when writing code. The
code files we ended up sticking with to help answer our business problem
can be found inside the folder titled "Finalized Code".

### Order of R Code Used

The R code files from the folder "Finalized Code" were used in the following order:

1)  initial_loading_and_cleaning.R (cleaning and merging all of the sensor readings data)
2)  merging_weather.R (cleaning and merging all of the weather data)
3)  imputing.R (imputes all missing values from the data set with the merged weather and sensor readings data)
4)  fault_event_creation.R (creates fault code events)
5)  combining_fault_events.R (merges the fault code events with the rest of the data)
6)  Exploratory Data Visualizations.R (exploratory analysis)
7)  Final Data Visualizations.R (multivariate visualizations)
8)  PredictiveModelingWithTurbineId.R (predictive modeling using the turbine ID as a predictor variable)
9)  ModelingWithoutTurbineId.R (predictive modeling where turbine ID is not used as a predictor variable)
10) ComparingModels.R (creating visualizations comparing the different predictive models)


### Requirements to Use the R Code

The following packages have been used for writing all our code:

1) ggplot2
2) lubridate
3) gridExtra
4) dplyr
5) hrbrthemes
6) magrittr
7) randomForest
8) pROC
9) imputeTS
10) MASS
11) rlist
12) e1071
13) caTools
14) class
15) tidyverse
16) RcolorBrewer
17) ggridges
18) viridis
19) ggExtra
20) hexbin


### Data Used

We used data provided by Daniel Madison
pertaining to fault codes, sensor readings, and weather.


### Prepared Data Set Used For Modeling

Using the data provided, we prepared our own data set to be used for
answering the business problem, which is called final_dataset.csv.
