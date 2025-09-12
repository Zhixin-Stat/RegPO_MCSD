# RegPO_MCSD
R codes for paper "Regression analysis of  misclassified current status data with potentially unknown test accuracy":

file: RegPO_MCSD is the main user-friendly function. By providing interested current status data with covariates X, test result y, obeservation time c, and setting sensitivity (alpha) = FALSE or a known number, specificity (beta) = FALSE or a known number, it can directly return you the covariate estimates (theta), their corresponding standard error (se.theta), and alpha and/or beta estimates with se.alpha and/or se.beta when either one or both are set to FALSE. The plot will report the estimated baseline cdf.

file: "Data.cvs" includes a simulated data set:
variable "observed.time" is c, "X1" and "X2" are covariates X, "test.result" is y.

file: Example.pdf generated using R Markdown, demonstrates the example analysis outputs obtained when applying the RegPO_MCSD function to Data.csv.

Note: the function will call packages "dlm", "stats", "MASS" and "coda".
