# Info about group software available from other repositories

# Table of Contents
1. [Program: codeml_SBA](#codeml_SBA)
2. [Program: codeml_ModL](#codeml_ModL)
3. [Tools: Protein stabilty simulation and analysis](#stabilty_tools)
4. [<font size ="6">Theory: Ecological Scaffold</font>](#ecological_scaffold)
<br/>

<a id="#codeml_SBA"></a>
## codeml_SBA

We developed an alternative to BEB called **smoothed bootstrap aggregation (SBA)**, for the inference of positively selected sites. SBA bootstraps site patterns from an alignment of protein coding DNA sequences to accommodate the uncertainty in the parameter estimates. Deriving the correction for parameter uncertainty from the data in hand, in combination with kernel smoothing techniques, improves site specific inference of positive selection. SBA is applicable to a wide variety of other inference problems in molecular evolution.

The code for SBA is derived from a forked version of codeml (by Ziheng Yang).  codeml_SBA was written by Joseph Mingrone while he was in the Bielawski Group.

The paper describing the method is:

>Mingrone, J., Susko, E., & Bielawski, J. (2016). Smoothed bootstrap aggregation for assessing selection pressure at amino acid sites. Molecular Biology and Evolution, 33(11), 2976-2989.

The repository for the code is: https://github.com/Jehops/codeml_sba

Please cite this paper if you use this repository.
<br/><br/>

<a id="#codeml_ModL"></a>
## codeml_ModL

Likelihood ratio tests are commonly used to test for positive selection acting on proteins. They are usually applied with thresholds for declaring a protein under positive selection determined from a chi-square or mixture of chi-square distributions. Although it is known that such distributions are not strictly justified due to the statistical irregularity of the problem, the hope has been that the resulting tests are conservative and do not lose much power in comparison with the same test using the unknown, correct threshold. We have shown that commonly used thresholds need not yield conservative tests, but instead give larger than expected Type I error rates. Statistical regularity can be restored by using a modified likelihood ratio test.

We introduce a modified LR test, which borrows from similar methods in mixture model tests of heterogeneity. The test statistic is obtained as it is for the standard LR test, but with the likelihood replaced by one that **penalizes** small mass on ω>1ω>1 relative to ω = 1. This strategy has been effective under a variety different mixture settings.

The paper describing the method is:

>Mingrone, J., Susko, E., & Bielawski, J. P. (2019). ModL: exploring and restoring regularity when testing for positive selection. Bioinformatics, 35(15), 2545-2554.

The code for the **penalized likelihood method** is derived from a forked version of codeml (by Ziheng Yang).  codeml_ModL was written by Joseph Mingrone while he was in the Bielawski Group.

The repository for the code is: https://github.com/Jehops/codeml_modl

Please cite this paper if you use this repository.
<br/><br/>


<a id="#stabilty_tools"></a>
## Protein Stabilty simulation and analysis tools 
Most proteins must fold into a native structure in which they are moderately stable before they are able to perform their biological function. Protein stability depends on the sequence of amino acids and their interactions in the folded three-dimensional structures. Because of these interactions, evolutionary selective constraints to maintain adequate stability result in epistatic dependencies between residues.  We developed and implemented mechanistic mutation-selection models in conjunction with a fitness framework derived from protein stability. We refer to these as the stability-informed site-dependent (S-SD) model and the stability-informed site-independent (S-SI) model that captures the average effect of stability constraints on individual sites of a protein.  We also used the stability-constrained mechanistic mutation-selection models to show that nonadaptive evolution can lead to both positive (Stokes) and negative (anti-Stokes) shifts in propensities following the fixation of an amino acid, emphasizing that the detection of negative shifts is not conclusive evidence of adaptation.

Distribution:
https://github.com/nooryoussef/antiStokes_shifts

https://github.com/nooryoussef/Consequences-of-stability-induced-epistasis

Citations:
>Youssef N, Susko E, Roger AJ, Bielawski JP. Evolution of Amino Acid Propensities under Stability-Mediated Epistasis. Mol Biol Evol. 2022 Mar 2;39(3):msac030. doi: 10.1093/molbev/msac030. PMID: 35134997; PMCID: PMC8896634.

>Youssef N, Susko E, Bielawski JP. Consequences of Stability-Induced Epistasis for Substitution Rates. Mol Biol Evol. 2020 Nov 1;37(11):3131-3148. doi: 10.1093/molbev/msaa151. PMID: 32897316.

Please cite these papers if you use these repositories.
<br/><br/>

<a id="#ecolgcial_scaffold"></a>
## Ecological scaffold theory

We designed **computer simulation of evolution in single populations and metapopulations motivated by a theoretical model**. These simulations show that although an altruistic mutant can be fixed within a single population of non-altruists by drift when nutrients are severely limited, the resulting altruistic population remains vulnerable to non-altruistic mutants. We then show how the imposition of the **ecological scaffold** onto a population of non-altruists alters the balance between selection and drift in a way that supports the fixation and subsequent persistence of altruism despite the possibility of invasion by non-altruists.

All simulations and calculations were implemented in MATLAB code version R2021a (by Christopher Jones as a postdoc in the Bielawski Group) under license number 861043 for academic use using custom scripts. 

The paper describing the method is:

>Jones, C. T., Meynell, L., Neto, C., Susko, E., & Bielawski, J. P. (2023). The role of the ecological scaffold in the origin and maintenance of whole-group trait altruism in microbial populations. BMC Ecology and Evolution, 23(1), 11.


The repository for the code is: https://github.com/cjones2DAL/WGT-Altruism-Model-Code/tree/v1.0

Please cite this paper if you use this repository.
<br/><br/>








