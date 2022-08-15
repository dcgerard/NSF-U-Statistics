
<!-- README.md is generated from README.Rmd. Please edit that file -->

# A U-statistic approach to population genetics

[![NSF-2132247](https://img.shields.io/badge/NSF-2132247-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=2132247)

This repository contains material based upon work supported by the
National Science Foundation under Grant
No. [2132247](https://nsf.gov/awardsearch/showAward?AWD_ID=2132247). The
opinions, findings, and conclusions or recommendations expressed are
those of the author and do not necessarily reflect the views of the
National Science Foundation.

## Manuscripts

-   Gerard (2022b): Read the paper
    [doi:10.1111/biom.13722](https://doi.org/10.1111/biom.13722) or the
    preprint version
    [bioRxiv:2021.09.24.461731](https://doi.org/10.1101/2021.09.24.461731)
    -   **Abstract**: Many bioinformatics pipelines include tests for
        equilibrium. Tests for diploids are well studied and widely
        available, but extending these approaches to autopolyploids is
        hampered by the presence of double reduction, the co-migration
        of sister chromatid segments into the same gamete during
        meiosis. Though a hindrance for equilibrium tests, double
        reduction rates are quantities of interest in their own right,
        as they provide insights about the meiotic behavior of
        autopolyploid organisms. Here, we develop procedures to (i) test
        for equilibrium while accounting for double reduction, and (ii)
        estimate the double reduction rate given equilibrium. To do so,
        we take two approaches: a likelihood approach, and a novel
        *U*-statistic minimization approach that we show generalizes the
        classical equilibrium chi-squared test in diploids. For small
        sample sizes and uncertain genotypes, we further develop a
        bootstrap procedure based on our *U*-statistic to test for
        equilibrium. We validate our methods on both simulated and real
        data.
-   Gerard (2022a): Read the preprint version
    [bioRxiv:2022.08.11.503635](https://doi.org/10.1101/2022.08.11.503635)
    -   **Abstract**: Hardy-Weinberg equilibrium is often explored to
        evaluate the assumption of random mating. However, in
        autopolyploids, organisms with more than two sets of homologous
        chromosomes, Hardy-Weinberg equilibrium and random mating are
        different hypotheses that require different statistical testing
        approaches. Currently, the only available methods to test for
        random mating in autopolyploids (i) heavily rely on asymptotic
        approximations and (ii) assume genotypes are known, ignoring
        genotype uncertainty. Furthermore, these approaches are all
        frequentist, and so do not carry the benefits of Bayesian
        analysis, including ease of interpretability, incorporation of
        prior information, and consistency under the null. Here, we
        present Bayesian approaches to test for random mating, bringing
        the benefits of Bayesian analysis to this problem. Our Bayesian
        methods also (i) do not rely on asymptotic approximations, being
        appropriate for small sample sizes, and (ii) optionally account
        for genotype uncertainty via genotype likelihoods. We validate
        our methods in simulations, and demonstrate on two real datasets
        how testing for random mating is more useful than testing for
        equilibrium (in a natural population) and testing for Mendelian
        segregation (in an experimental S1 population). Our methods are
        implemented in Version 2.0.0 of the hwep R package on GitHub
        <https://github.com/dcgerard/hwep>.

## Software

-   The `hwep` R package: <https://cran.r-project.org/package=hwep>
    -   Inference concerning equilibrium and random mating in
        autopolyploids. Methods are available to test for equilibrium
        and random mating at any even ploidy level (\>2) in the presence
        of double reduction at biallelic loci. For autopolyploid
        populations in equilibrium, methods are available to estimate
        the degree of double reduction. We also provide functions to
        calculate genotype frequencies at equilibrium, or after one or
        several rounds of random mating, given rates of double
        reduction. You can read about these methods in Gerard (2022b)
        and Gerard (2022a).
-   The `phwelike` R package
    ([doi:10.5281/zenodo.5531955](https://doi.org/10.5281/zenodo.5531955)):
    <https://github.com/dcgerard/phwelike>
    -   This package takes the methods developed and written by Jiang,
        Ren, and Wu (2021) and implements them in the form of an R
        package. This will allow researchers, such as myself, to better
        compare our methods against those of Jiang, Ren, and Wu (2021).

## Reproducible Research

-   Results from Gerard (2022b)
    ([doi:10.5281/zenodo.5531872](https://doi.org/10.5281/zenodo.5531872)):
    <https://github.com/dcgerard/hwesims>
    -   This code repository contains all the scripts necessary to
        reproduce the results from Gerard (2022b). We emphasize extreme
        reproducibilty by providing executable, and linked, code and
        data.
-   Results from Gerard (2022a):
    <https://github.com/dcgerard/rmbayes_sims>
    -   This code repository reproduces all of the results from Gerard
        (2022a), including simulations and real-data analyses.

## Presentations

-   [doi:10.5281/zenodo.5589844](https://doi.org/10.5281/zenodo.5589844):
    Slides for a presentation at the American University Department of
    Mathematics and Statistics Colloquium on 2021-10-19. This work is
    based on Gerard (2022b).
-   [PAG 2022
    Poster](https://pag.confex.com/pag/xxix/meetingapp.cgi/Paper/43285):
    Virtual poster presentation at the 2022 Plant & Animal Genome
    Conference.
-   [JSM 2022 Poster](https://doi.org/10.5281/zenodo.6987179): This
    poster was presented by D. Thomas Scartz at the 2022 Joint
    Statistical Meetings in Washington, DC. You can see the abstract for
    the poster
    [here](https://ww2.amstat.org/meetings/jsm/2022/onlineprogram/AbstractDetails.cfm?abstractid=322319).

## Education Materials

-   [Advanced R Course Materials](https://dcgerard.github.io/advancedr/)
    -   This course prepares students for software development using the
        R statistical programming language. Topics include: version
        control via git and its command line interface, package
        development, unit testing, base R data structures, environments,
        object oriented programming via S3 and S4, metaprogramming,
        interfacing with C++ via Rcpp, parallel processing with futures,
        and batch scheduling jobs via LSF. This course was taught during
        the Spring semester of 2022 at American University. All
        materials that I created for this course are under a CC BY-NC
        4.0 license, so you are free to use them for non-commercial
        purposes as long as you provide attribution.
-   [Genetic Data Analysis](https://dcgerard.github.io/gda/)
    -   This website contains a series of hand-written lecture notes I
        created for my research group on basic genetic data analysis.
        Topics include genotype and allele frequency estimation,
        Hardy-Weinberg equilibrium testing, linkage disequilibrium
        testing and estimation, maximum likelihood estimation and the
        expectation-maximization algorithm, basic Bayesian inference,
        genetic drift and mutation (including in the context of
        molecular evolution), coalescent theory, inbreeding, and
        population subdivision. I also have a few lectures on classic
        research papers. This material is under a CC BY-NC 4.0 license,
        so you can use them for non-commercial purposes as long as you
        provide attribution.

## References

<div id="refs" class="references csl-bib-body hanging-indent">

<div id="ref-gerard2022bayesian" class="csl-entry">

Gerard, David. 2022a. “Bayesian Tests for Random Mating in
Autopolyploids.” *bioRxiv*. <https://doi.org/10.1101/2022.08.11.503635>.

</div>

<div id="ref-gerard2022double" class="csl-entry">

———. 2022b. “Double Reduction Estimation and Equilibrium Tests in
Natural Autopolyploid Populations.” *Biometrics* In press.
<https://doi.org/10.1111/biom.13722>.

</div>

<div id="ref-jiang2021computational" class="csl-entry">

Jiang, Libo, Xiangyu Ren, and Rongling Wu. 2021. “Computational
Characterization of Double Reduction in Autotetraploid Natural
Populations.” *The Plant Journal* 105 (6): 1703–9.
<https://doi.org/10.1111/tpj.15126>.

</div>

</div>
