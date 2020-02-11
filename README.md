# Continuous-Soil-Properties project
Prediction of continuous soil properties at 30m resolution for the Continental USA

# Properties to be predicted
Property     | Units         | Notes
------------ | ------------- | -------------
Clay | g/kg or % |
Sand | g/kg or % |
Silt | g/kg or % |
Depth| cm        |
pH | unitless    |
rock fragments   | (m3 m-3)
Available water capacity | (mm mm-1 ?) | probably need to run Rosetta or Saxton and Rawls

# Potential properties to be predicted
Property     | Units         | Notes
------------ | ------------- | -------------
ECEC | (cmolc/kg) |
N | (%) |
C | (%) |
electrical conductivity | (dS/m) |


# Semi-detailed Structure of Project. 

## A. Pedon Data Cleaning and Prep per Dataset [per property?]
### A.1 Forest Service NRM data
### A.2 NASIS point data
### A.3 KSSL data
### A.4 RaCA
### A.5 Other point data

## B. Depth Harmonization (0-5, 5-15, 15-30, 30-60, 60-100, 100-200 cm)  [per property]

## C. Build Regression Matrix 
### C.1 Extract DEM derivatives
### C.2 Extract spectral derivatives
### C.3 Extract other geospatial covariates

## D. Build Models [per property]
### D.1 Build list to hold each regional model per property [big point of discussion here]
### D.2 Set up training routine (cross validation repeated 10 times or something). 
### D.3 Training/evaluation data split
### D.4 Build continental model
### D.5 Build regional models

## E. Model Evaluation
### E.1 Evalute contiental model
### E.2 Evaulate each regional model 
### E.3 Covariate importance

## F. Spatial Predictions [how to use regional models?]

## G. Spatial Uncertainty

## H. Locations where the addition of legacy or new sample data would prove most beneficial to model improvement and/or uncertainty reduction. 
