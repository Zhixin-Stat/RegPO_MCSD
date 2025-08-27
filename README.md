# MisCurrentPO
R codes for paper "Regression analysis of  misclassified current status data with potentially unknown test accuracy":

file: MisCrrentPO_function is the main user-friendly function. By providing interested current status data with covariates X, test result y, obeservation time c, and setting sensitivity (alpha) = FALSE or a known number, specificity (beta) = FALSE or a known number, it can directly return you the covariate estimates (theta), their corresponding standard error (se.theta), and alpha and/or beta estimates with se.alpha and/or se.beta when either one or both are set to FALSE.  


Below codes are clean version for developer,if you are interested in reporducing the results:

file: MIspline.R can be saved in a separate R file and then call it in below two files by source("MIspline.R")

file: known_sesp, main code for the case that data have known sensitivity and specificity. This code is used for data simulation section. 

file: unknown_se, an example main code for the case that study == 1 has unknown sensitivity and study != 1 has known sensitivity, while specificity is known across all the studies. This code is used to generate outputs for RFTS fibroid real data analysis section.
