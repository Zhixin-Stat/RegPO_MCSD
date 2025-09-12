# RegPO_MCSD
R codes for paper "Regression analysis of  misclassified current status data with potentially unknown test accuracy":

file: RegPO_MCSD is the main user-friendly function. By providing interested current status data with covariates X, test result y, obeservation time c, and setting sensitivity (alpha) = FALSE or a known number, specificity (beta) = FALSE or a known number, it can directly return you the covariate estimates (theta), their corresponding standard error (se.theta), and alpha and/or beta estimates with se.alpha and/or se.beta when either one or both are set to FALSE.  

file: "Data.cvs" includes a simulated data set (It is genearated from survival function S(t|X1, X2)={1+Lambda_0(t)exp(\theta_1 X_{i1}+\theta_2 X_{i2})}^(-1), i=1,...,n, n=200, where X_1 is a Bernoulli random variable with a probability of success 0.5, and X_2 is a normal random variable with mean 0 and variance 0.25, The true baseline odds function is set to be Lambda_0(t)=t^3+t, and the true values of \theta_1 = 1, \theta_2 = -1, sensitivity (\alpha) = 0.90, specificity (\beta) = 0.90.)
variable "observed.time" is c, "X1" and "X2" are covariates X, "test.result" is y.

file: example illustrates the analysis output after applying the RegPO_MCSD function to the Data.cvs
