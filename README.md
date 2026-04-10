# Overview
This repository contains the code and data used in our study:  
**"Machine Learning-Based Precise Flow Synthesis of Platinum-Group-Metal High-Entropy Alloy Nanoparticles".**  
  
It provides a precise synthesis method for homogeneously alloyed and size-controlled RuRhPdIrPt HEA NPs by integrating flow synthesis with interpretable machine learning.  
  
This repository includes:
  
1. **Decision tree classification (DTC, DTC_DCV)**  
DTC model with and without double cross-validation to evaluate synthesis conditions for obtaining non-agglomerated and homogeneously alloyed HEA NPs.  
2. **Partial least squares regression (PLS_DCV_CVPFI)**  
PLS regression model with double cross-validation to evaluate:  
&nbsp;&nbsp;- predictive performance of particle sizes  
&nbsp;&nbsp;- regression coefficients   
&nbsp;&nbsp;- cross-validated permutation feature importances (CVPFI)  

## Repository structure
FR_ML/  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Data/&nbsp;&nbsp;&nbsp;&nbsp;# Input datasets  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Agglomerate/  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Composition/  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;LatticeConstant/  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;MeanSize/  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Notebooks/&nbsp;&nbsp;&nbsp;&nbsp;# Jupyter notebooks for reproducing analyses and figures  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;README.md  

## Requirements
- Python 3.10 or later  
- NumPy  
- Pandas  
- Scikit-learn  
- DCEkit  

## Note
Analyses were performed on Windows.  
The code has not been tested on Linux or macOS environments. 

## Author
- Daiki Takahashi
- Hiromasa Kaneko
