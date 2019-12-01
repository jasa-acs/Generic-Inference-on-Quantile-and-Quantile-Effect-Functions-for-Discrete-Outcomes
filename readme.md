# Generic Inference on Quantile and Quantile Effect Functions for Discrete Outcomes

# Author Contributions Checklist Form

## Data

### Abstract

1) Oregon health insurance experiment: In 2008, Oregon implemented a limited expansion of itsMedicaid program for low-income adults through a lottery, selecting names from a waiting list tofill a limited number of available spots. Those selected had the opportunity to apply for Medicaidand to enroll if they met eligibility requirements. This lottery presented a unique opportunity togauge the effects of Medicaid using the rigorous standard of a randomized controlled trial.

2) The US Collaborative Perinatal Project (CPP) includes over 31,000 women who gave birth in12 medical centers between 1959 and 1965. All medical centers were in urban areas: six in theNortheast, four in the South, one in the West, and one in the north-central region of the UnitedStates. Some institutions selected all eligible women, while others took a random sample. Thesocioeconomic and ethnic composition of the participants is representative of the populationqualifying for medical care at the participating institutions. These women were resurveyed whentheir children were eight months, four years, and seven years old.


### Availability

Both datasets are publicly available.

### Description

The Oregon datasets is available at http://www.nber.org/oregon/4.data.html.

The CPP dataset is available at dx.doi.org/10.1257/aer.103.2.981.

Both datasets are saved using the .dta Stata format.

Data dictionaries are available with the datasets at the above mentioned links. Descriptive statistics and additional information are available in the following research papers (and their appendices) that used the same datasets: 

1) Finkelstein, A., Taubman, S., Wright, B., Bernstein, M., Gruber, J., Newhouse, J. P., Allen, H., Baicker, K. and Group, O. H. S. (2012), ‘The oregon health insurance experiment: Evidence from the first year’, The Quarterly Journal of Economics 127(3), 1057–1106. 

2) Fryer Jr, R. G. and Levitt, S. D. (2013), ‘Testing for racial differences in the mental ability of young children’, The American Economic Review 103(2), 981–1005.

## Code

### Abstract

We provide an R package (discreteQ) that implement the algorithms defined in our paper. The latest updated version of the package can be installed from the Github depository “bmelly/discreteQ”. The help files as well as the vignette included in the package give numerous examples. In addition, the available R codes apply the commands in the package to generate all the results of the paper (both applications and the simulations in the supplementary appendix).

### Description

The R codes have been uploaded at Github: https://github.com/bmelly/discreteQ. They have the following DOI: doi.org/10.5281/zenodo.1406948. This repository contains the source codes for the R package 'discreteQ' as well as (in the folder 'replication') the data and codes that allow replicating the empirical and simulation results presented in the paper.

Licensing information: MIT License

### Supporting software requirements

We performed the analysis presented in the manuscript with R version 3.5.2 and the following R libraries: discreteQ (0.3.0), foreign (0.8-71), doParallel (1.0.14), doRNG (1.7.1), xtable (1.8-3), Hmisc (4.2-0), foreach (1.4.4), iterators (1.0.10), plyr (1.8.4), rngtools (1.3.1), and codetools (0.2-16).


## Instructions for Use

### Reproducibility

All results in the paper and the supplementary appendix can be replicated with the provided codes, data and R package. See the README file for the details. Note that some results take a very long time to be computed (up to 10 days for the second application). The approximate computing time for each figure is given in the master code file. Note that the computing time for the second application is particularly long because the sample size, the number of covariates, the number of distinct values taken by the outcome and the number of bootstrap replications are all relatively high (almost 30'000 observations, 247 covariates, 128 distinct values, 1000 bootstrap replications).
