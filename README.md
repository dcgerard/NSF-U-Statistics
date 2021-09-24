
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

-   Gerard (2021): Read the paper here: \[URL TO BE Provided\]
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
        estimate double reduction given equilibrium. To do so, we take
        two approaches: a likelihood approach, and a novel U-statistic
        minimization approach that we show generalizes the classical
        equilibrium χ-squared test in diploids. For small sample sizes
        and uncertain genotypes, we further develop a bootstrap
        procedure based on our U-statistic to test for equilibrium.
        Finally, we highlight the difficulty in distinguishing between
        random mating and equilibrium in tetraploids at biallelic loci.
        Our methods are implemented in the hwep R package on GitHub
        <https://github.com/dcgerard/hwep>.

## Software

-   The `hwep` R package: <https://github.com/dcgerard/hwep>
    -   Inference concerning equilibrium and random mating in
        autopolyploids. Methods are available to test for equilibrium
        and random mating at any even ploidy level (&gt;2) in the
        presence of double reduction at biallelic loci. For
        autopolyploid populations in equilibrium, methods are available
        to estimate the degree of double reduction. We also provide
        functions to calculate genotype frequencies at equilibrium, or
        after one or several rounds of random mating, given rates of
        double reduction. You can read about these methods in
        Gerard (2021).
-   The `phwelike` R package: <https://github.com/dcgerard/phwelike>
    -   This package takes the methods developed and written by Jiang,
        Ren, and Wu (2021) and implements them in the form of an R
        package. This will allow researchers, such as myself, to better
        compare our methods against those of Jiang, Ren, and Wu (2021).

## Reproducible Research

-   <https://github.com/dcgerard/hwesims>: This code repository contains
    all the scripts necessary to reproduce the results from
    Gerard (2021). We emphasize extreme reproducibilty by providing
    executable, and linked, code and data.

## Education Materials

## References

<div id="refs" class="references csl-bib-body hanging-indent">

<div id="ref-gerard2021double" class="csl-entry">

Gerard, David. 2021. “Double Reduction Estimation and Equilibrium Tests
in Natural Autopolyploid Populations.” *Unpublished Manuscript*.

</div>

<div id="ref-jiang2021computational" class="csl-entry">

Jiang, Libo, Xiangyu Ren, and Rongling Wu. 2021. “Computational
Characterization of Double Reduction in Autotetraploid Natural
Populations.” *The Plant Journal* 105 (6): 1703–9.
<https://doi.org/10.1111/tpj.15126>.

</div>

</div>
