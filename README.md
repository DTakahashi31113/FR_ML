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
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;data/&nbsp;&nbsp;&nbsp;&nbsp;# Input datasets  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Agglomerate/  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Composition/  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;LatticeConstant/  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;MeanSize/  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;notebooks/&nbsp;&nbsp;&nbsp;&nbsp;# Jupyter notebooks for reproducing analyses and figures  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;README.md  

## Requirements  
- Python 3.10+  
- NumPy  
- Pandas  
- Scikit-learn  
- DCEkit  

## Instructions  
1. Install requirements  
2. Run the scripts below to reproduce the figures.

## Dataset-script correspondence 
### Agglomeration analysis  
Dataset:  
&nbsp;- data/Agglomerate/*.csv  
Scripts:  
&nbsp;- DTC.py  
&nbsp;- DTC_DCV.py  
Outputs:  
&nbsp;- Figure 2  
&nbsp;- Supplementary Figure 3  

### Composition analysis  
Dataset:  
&nbsp;- data/Composition/*.csv  
Scripts:  
&nbsp;- DTC.py  
&nbsp;- DTC_DCV.py  
Outputs:  
&nbsp;- Figure 3a–c  
&nbsp;- Supplementary Figures 4–8  

### Lattice constant analysis  
Dataset:  
&nbsp;- data/LatticeConstant/*.csv  
Scripts:  
&nbsp;- DTC.py  
&nbsp;- DTC_DCV.py  
Outputs:  
&nbsp;- Figure 3d–f  
&nbsp;- Supplementary Figures 9–14  

### Particle size analysis  
Dataset:  
&nbsp;- data/MeanSize/HEA25_A.csv  
Script:  
&nbsp;- PLS_DCV_CVPFI.py  
Output:  
&nbsp;- Figure 5  

## Note  
Analyses were performed on Windows.  
The code has not been tested on Linux or macOS environments. 

## Authors
- Daiki Takahashi
- Hiromasa Kaneko
