# Informative Horseshoe Bayesian prior and Shapley values to facilitate RuleFit interpretability

## Info

Leiden University's Statistics and Data Science programme  
**Master's Thesis**  
**Student:** Giorgio Spadaccini  
**Supervisors:** Mark van de Wiel, Marjolein Fokkema  

## Prerequisites

- The package _infHS_ from https://github.com/cbusatto/infHS needs to be installed
- The package _horserule_ from https://github.com/mattiasvillani/horserule/ needs to be installed
- The packages _pre,ggplot2,ggthemes,ggforce,MASS,randcorr,partykit,glmnet,stringr,dplyr,patchwork,Matrix,data.table,randomForest,xgboost_ and _horseshoe_ from CRAN need to be installed, together with all their requirements

## Running the code

The code is divided into three folders, each for a different dataset on which the informative Horseshoe RuleFit is tried: Friedman 1, Extra dataset, and Helius dataset.

- For the two synthetic datasets Friedman 1 and Extra, the code is split into two files: the file _Simulation.Rmd_ generates the data and fits all models on it. The file _Comparison.Rmd_ uses the fitted models produced from the _Simulation.Rmd_ file to compare the quality of fit and the importance measures.
- For the Helius dataset, all code is in the _Code.Rmd_ file. The code is provided but cannot be run without data, for which access needs to be requested.

All model fits and computationally intense intermediate objects are saved in _.Rda_ files. The code currently avoids re-generating any of these objects. In order to enforce generating them from scratch, remove _eval=F_ from the code chunks that generate them.

## Data

The dataset from the Helius study is not available to the public, and is therefore not included in the repository. The synthetic datasets and their generating functions discussed on Chapter 4 are available and can be used to reproduce the code.
