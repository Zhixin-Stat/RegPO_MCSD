# RegPO_MCSD
R codes for paper "Regression analysis of  misclassified current status data with potentially unknown test accuracy":

RegPO_MCSD is the main user-friendly function. Given current status data with covariates X, test results y, observation time c, and user-specified sensitivity (alpha) and specificity (beta) values (either FALSE or a known number), the function returns covariate estimates (theta) with their standard errors (se.theta). If alpha and/or beta are set to FALSE, it also estimates them along with se.alpha and/or se.beta. The output includes a plot of the estimated baseline CDF.

file: "Data.cvs" includes a simulated data set:
variable "observed.time" is c, "X1" and "X2" are covariates X, "test.result" is y.

file: Example.pdf generated using R Markdown, demonstrates the example analysis outputs obtained when applying the RegPO_MCSD function to Data.csv.

Note: the function will call packages "dlm", "stats", "MASS" and "coda".
