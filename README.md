# MisCurrentPO
R codes for paper "Regression analysis of  misclassified current status data with potentially unknown test accuracy".

file: MIspline.R can be saved in a separate R file and then call it in main code by source("MIspline.R")

file: known_sesp, main code for the case that data have known sensitivity and specificity. This code is used in data simulation section. 

file: unknown_se, an example main code for the case that study == 1 has unknown sensitivity and study != 1 has known sensitivity, while specificity is known across all the studies. This codes is used to generate outputs for RFTS fibroid real data analysis in the paper. 
