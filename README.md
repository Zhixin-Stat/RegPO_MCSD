# RegPO_MCSD
R codes for paper "Regression analysis of  misclassified current status data with potentially unknown test accuracy":

RegPO_MCSD is the main user-friendly function. Given current status data with covariates X, test results y, observation time c, and user-specified sensitivity (alpha) and specificity (beta) values (either FALSE or a known number), the function returns covariate estimates (theta) with their standard errors (se.theta). If alpha and/or beta are set to FALSE, it also estimates them along with se.alpha and/or se.beta. The variance estimation is obtained by outer product of gradients (OPG) method for simplicity in this package. The output includes a plot of the estimated baseline CDF.

file: "Data.cvs" includes a simulated data set:
variable "observed.time" is c, "X1" and "X2" are covariates X, "test.result" is y.

file: Example.pdf generated using R Markdown, demonstrates the example analysis outputs obtained when applying the RegPO_MCSD function to Data.csv.

Note: 

1. The function will call packages "dlm", "stats", "MASS" and "coda".

2. The variance estimates of the parameters can also be obtained by inverting the observed information matrix, as described in the paper. The corresponding R code will be made available in the near future or upon request. Additional details comparing the three variance estimation methods the Louis method, the outer product of gradients (OPG) method, and the observed information matrix (OIM) method can be found in Appendix Table C.1 of the paper.
