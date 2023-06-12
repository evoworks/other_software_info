# Info about group software available from other repositories

## codeml_SBA

We developed an alternative to BEB called **smoothed bootstrap aggregation (SBA)**, for the inference of positively selected sites. SBA bootstraps site patterns from an alignment of protein coding DNA sequences to accommodate the uncertainty in the parameter estimates. Deriving the correction for parameter uncertainty from the data in hand, in combination with kernel smoothing techniques, improves site specific inference of positive selection. SBA is applicable to a wide variety of other inference problems in molecular evolution.

The code for SBA is derived from a forked version of codeml (by Ziheng Yang).  codeml_SBA was written by Joseph Mingrone while he was in the Bielawski Group.

The paper describing the method is:

>Mingrone, J., Susko, E., & Bielawski, J. (2016). Smoothed bootstrap aggregation for assessing selection pressure at amino acid sites. Molecular Biology and Evolution, 33(11), 2976-2989.

The repository for the code is: https://github.com/Jehops/codeml_sba

Please cite this paper if you use this repository.


## codeml_ModL

Likelihood ratio tests are commonly used to test for positive selection acting on proteins. They are usually applied with thresholds for declaring a protein under positive selection determined from a chi-square or mixture of chi-square distributions. Although it is known that such distributions are not strictly justified due to the statistical irregularity of the problem, the hope has been that the resulting tests are conservative and do not lose much power in comparison with the same test using the unknown, correct threshold. We have shown that commonly used thresholds need not yield conservative tests, but instead give larger than expected Type I error rates. Statistical regularity can be restored by using a modified likelihood ratio test.

We introduce a modified LR test, which borrows from similar methods in mixture model tests of heterogeneity. The test statistic is obtained as it is for the standard LR test, but with the likelihood replaced by one that **penalizes** small mass on ω>1ω>1 relative to ω = 1. This strategy has been effective under a variety different mixture settings.

The paper describing the method is:

>Mingrone, J., Susko, E., & Bielawski, J. P. (2019). ModL: exploring and restoring regularity when testing for positive selection. Bioinformatics, 35(15), 2545-2554.

The code for the **penalized likelihood method** is derived from a forked version of codeml (by Ziheng Yang).  codeml_ModL was written by Joseph Mingrone while he was in the Bielawski Group.

The repository for the code is: https://github.com/Jehops/codeml_modl

Please cite this paper if you use this repository.










