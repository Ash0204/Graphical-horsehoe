# DESCRIPTION
Draw Monte Carlo samples from the posterior distribution under the graphical horseshoe prior, to estimate the precision matrix for multivariate Gaussian data.

# ARGUMENTS
S -Y'*Y : sample covariance matrix * n (symmetric)
n -Sample size
burnin -number of MCMC burnins
nmc -number of MCMC saved samples

# DETAILS
Draw posterior samples to estimate the precision matrix for multivariate Gaussian data. Posterior means of the samples is the graphical horseshoe estimate by Li, Bhadra and Craig (2017). The function uses matrix decomposition and variable change from the Bayesian graphical lasso by Wang (2012), and the variable augmentation for sampling under the horseshoe prior by Makalic and Schmidt (2016). Structure of the graphical horseshoe function GHS.m was inspired by the Bayesian graphical lasso function using blocked sampling BayesGLassoGDP.m, authored by Wang (2012).

# REFERENCES
Yunfan Li, Anindya Bhadra and Bruce A. Craig (2017). The graphical horseshoe estimator for inverse covariance matrices. Wang, H. (2012). Bayesian graphical lasso models and efficient posterior computation. Bayesian Analysis, 7(4):867-886. Makalic, E. and Schmidt, D. F. (2016). A simple sampler for the horseshoe estimator. IEE Signal Processing Letters, 23(1):179-182
