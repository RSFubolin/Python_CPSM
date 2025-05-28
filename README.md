# Python_CPSM
A constrained PROSAIL-PRO spectra matching approach for extension of multispectral reflectance.

# Getting Started
To set the absolute pathname of input data and output data and running follow these simple example steps

## Prerequisites
 The CPSM is built with python based on Jupyter Notebook.You need some basic python packages: numpy, pandas, scikit-learn, operator, tqdm.

## Download the sample Input data
We provides a examples data which simulated using prospect-pro and 4 SAIL. The file can be downloaded from the following link: https://pan.baidu.com/s/1H3zAq-_I__Kl7ZxfD7LzJQ?pwd=nsic, which password is "nsic". In fact, the input data can be other reflectance simulated using radiative transfer models of vegetation. The P4Mdata.cvs is the spectral reflectance of multispectral unmanned aerial vehicles, which includs measured leaf area index (LAI), protein, chlorophyll content(chl), and the reflectance (blue, green, red, red_edge, nir). The ConstrainParameter.csv is the data for constrainning to match spectra, including LAI, chl, and equivalent water thickness.

## Setting the path of input and output in the code
If you extract the .zip to D, you can set D:\CPSM\data\Directional_reflectance_allband.csv. This file can be obtained from the above link.

## Description
The results go to the "results" folder, when the CPSM has been completed. The examples of the results can be seen in the results_spectral400nm_2500nm.csv, which includs spectral reflectance at 400 ~ 2500 nm with 1nm spectral resolution corresponds to each pixel. The process results will be saved in a folder, named "LUT20%". The files in LUT folder are the optimal solution space for matching. The files in RMSE folder are the matching accuracy. If you don not want to generate these intermediate process files, you can improve the source code. Because this intermediate process file occupy relatively large space.

## Statement
The CPSM cannot be used for any commercial purposes without the author's consent. If you used the CPSM including modification, improvement and publish paper, place cite the following paper. 

# Contact
Bolin Fu: fubolin@glut.edu.cn
Zhinan Lao: 2120211864@glut.edu.cn
