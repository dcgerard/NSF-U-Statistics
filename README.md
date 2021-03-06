
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

-   Gerard (2022): Read the paper
    [doi:10.1111/biom.13722](https://doi.org/10.1111/biom.13722) or the
    preprint version
    [bioRxiv:10.1111/biom.13722](https://doi.org/10.1101/2021.09.24.461731)
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
        reduction. You can read about these methods in Gerard (2022).
-   The `phwelike` R package
    ([doi:10.5281/zenodo.5531955](https://doi.org/10.5281/zenodo.5531955)):
    <https://github.com/dcgerard/phwelike>
    -   This package takes the methods developed and written by Jiang,
        Ren, and Wu (2021) and implements them in the form of an R
        package. This will allow researchers, such as myself, to better
        compare our methods against those of Jiang, Ren, and Wu (2021).

## Reproducible Research

-   Results from Gerard (2022)
    ([doi:10.5281/zenodo.5531872](https://doi.org/10.5281/zenodo.5531872)):
    <https://github.com/dcgerard/hwesims>
    -   This code repository contains all the scripts necessary to
        reproduce the results from Gerard (2022). We emphasize extreme
        reproducibilty by providing executable, and linked, code and
        data.

## Presentations

-   [doi:10.5281/zenodo.5589844](https://doi.org/10.5281/zenodo.5589844):
    Slides for a presentation at the American University Department of
    Mathematics and Statistics Colloquium on 2021-10-19. This work is
    based on Gerard (2022).
-   [PAG 2022
    Poster](https://pag.confex.com/pag/xxix/meetingapp.cgi/Paper/43285):
    Virtual poster presentation at the 2022 Plant & Animal Genome
    Conference.

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

## References

<div id="refs" class="references csl-bib-body hanging-indent">

<div id="ref-gerard2022double" class="csl-entry">

Gerard, David. 2022. “Double Reduction Estimation and Equilibrium Tests
in Natural Autopolyploid Populations.” *Biometrics* In press.
<https://doi.org/10.1111/biom.13722>.

</div>

<div id="ref-jiang2021computational" class="csl-entry">

Jiang, Libo, Xiangyu Ren, and Rongling Wu. 2021. “Computational
Characterization of Double Reduction in Autotetraploid Natural
Populations.” *The Plant Journal* 105 (6): 1703–9.
<https://doi.org/10.1111/tpj.15126>.

</div>

</div>
