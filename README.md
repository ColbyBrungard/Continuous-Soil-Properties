#Continuous-Soil-Properties
Prediction of continuous soil properties at 30m resolution for CONUS

# Properties to be predicted
Property     | Units         | Notes
------------ | ------------- | -------------
Clay | g/kg or % |
Sand | g/kg or % |
Silt | g/kg or % |
Depth| cm        |
pH | unitless    |
rock fragments   | (m3 m-3)
Available water capacity | (mm mm-1 ?) | probably need to run Rosetta or Saxton and Rawls, or something on sand and clay predictions rather than running on pedon data and trying to model AWC [super open to discussion]

# Pptential properties to be predicted
Property     | Units         | Notes
------------ | ------------- | -------------
ECEC | (cmolc/kg) |
N | (%) |
C | (%) |
electrical conductivity | (dS/m) |


## Semi-detailed Structure of Project. I'm sort of envisioning that each bullet point will have it's own script that does only that task.


##A. Pedon data Cleaining and Prep per Dataset [per property?]
###Forest Service NRM data
###NASIS point data
###KSSL data
###RaCA
###Other point data


## B. Depth Harmonization [per property] (0-5, 5-15, 15-30, 30-60, 60-100, 100-200 cm)

## C. Build Regression Matrix 
### Extract DEM derivatives
### Extract spectral derivatives
### Extract other geospatial covariates

## D. Build Models [per property]
### Build list to hold each regional model per property [big point of discussion here]
### Set up training routine (cross validation repeated 10 times or something). 
### Training/evaluation data split
### Build continental model
    #### Exploratory data analysis [per property - should be on-going during data cleaning etc.]
### Build regional models
    #### Exploratory data analysis [per region]

## E. Model Evaluation
### Evaulate each regional model 
### Covariate importance

## F. Prediction [how to use regional models?]

## G. Spatial Uncertainty

## H. Locations where the addition of legacy or new sample data would prove most beneficial to model improvement and/or uncertainty reduction. 
