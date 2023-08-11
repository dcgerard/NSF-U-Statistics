
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

- Gerard (2022c): Read the paper
  [doi:10.1111/biom.13722](https://doi.org/10.1111/biom.13722) or the
  preprint version
  [bioRxiv:2021.09.24.461731](https://doi.org/10.1101/2021.09.24.461731)
  - **Abstract**: Many bioinformatics pipelines include tests for
    equilibrium. Tests for diploids are well studied and widely
    available, but extending these approaches to autopolyploids is
    hampered by the presence of double reduction, the co-migration of
    sister chromatid segments into the same gamete during meiosis.
    Though a hindrance for equilibrium tests, double reduction rates are
    quantities of interest in their own right, as they provide insights
    about the meiotic behavior of autopolyploid organisms. Here, we
    develop procedures to (i) test for equilibrium while accounting for
    double reduction, and (ii) estimate the double reduction rate given
    equilibrium. To do so, we take two approaches: a likelihood
    approach, and a novel *U*-statistic minimization approach that we
    show generalizes the classical equilibrium chi-squared test in
    diploids. For small sample sizes and uncertain genotypes, we further
    develop a bootstrap procedure based on our *U*-statistic to test for
    equilibrium. We validate our methods on both simulated and real
    data.
- Gerard (2022a): Read the preprint version
  [bioRxiv:2022.08.11.503635](https://doi.org/10.1101/2022.08.11.503635)
  - **Abstract**: Hardy-Weinberg proportions (HWP) are often explored to
    evaluate the assumption of random mating. However, in
    autopolyploids, organisms with more than two sets of homologous
    chromosomes, HWP and random mating are different hypotheses that
    require different statistical testing approaches. Currently, the
    only available methods to test for random mating in
    autopolyploids (i) heavily rely on asymptotic approximations
    and (ii) assume genotypes are known, ignoring genotype uncertainty.
    Furthermore, these approaches are all frequentist, and so do not
    carry the benefits of Bayesian analysis, including ease of
    interpretability, incorporation of prior information, and
    consistency under the null. Here, we present Bayesian approaches to
    test for random mating, bringing the benefits of Bayesian analysis
    to this problem. Our Bayesian methods also (i) do not rely on
    asymptotic approximations, being appropriate for small sample sizes,
    and (ii) optionally account for genotype uncertainty via genotype
    likelihoods. We validate our methods in simulations, and demonstrate
    on two real datasets how testing for random mating is more useful
    for detecting genotyping errors than testing for HWP (in a natural
    population) and testing for Mendelian segregation (in an
    experimental S1 population). Serendipitously, we further show that
    our tests for random mating in autopolyploids may also be applied as
    tests for HWP in allopolyploids. Our methods are implemented in
    Version 2.0.2 of the `hwep` R package on the Comprehensive R Archive
    Network <https://cran.r-project.org/package=hwep>.
- Gerard (2022b): Read the paper
  [doi:10.3389/fgene.2022.1027209](https://doi.org/10.3389/fgene.2022.1027209)
  or the preprint version
  [HAL:hal-03754674](https://hal.archives-ouvertes.fr/hal-03754674)
  - **Abstract**: Three similar manuscripts, by many of the same
    authors, were recently published describing methods for
    Hardy-Weinberg equilibrium and random mating testing in
    autotetraploids \[Sun, et al. *Trends in Genetics*, 37(6), 2021.
    [doi:10.1016/j.tig.2020.11.006](https://doi.org/10.1016/j.tig.2020.11.006)\],
    autohexaploids \[Wang, et al. *Horticulture Research*, 9, 2022.
    [doi:10.1093/hr/uhac104](https://doi.org/10.1093/hr/uhac104)\], and
    autooctoploids \[Wang, et al. *Frontiers in Genetics*, 12, 2021.
    [doi:10.3389/fgene.2021.794907](https://doi.org/10.3389/fgene.2021.794907)\].
    We found issues with these manuscripts, which we detail here. The
    main problems that we see are (i) extensive mistakes and
    implementation errors, (ii) confusion between random mating and
    equilibrium, (iii) confusion between allo- and autopolyploid
    inheritance, and (iv) poor hypothesis testing approaches. We provide
    examples and simulations when appropriate. All of our results are
    open and reproducible.

## Master’s Theses:

- Matoka Nana (2023): Read the thesis
  [doi:10.57912/23504199](https://doi.org/10.57912/23504199) or
  [ProQuest:2808426065](https://www.proquest.com/docview/2808426065)
  - **Abstract**: In statistical genetics, a common task is to evaluate
    the assumption of random mating, which is a baseline for population
    genetic models and can be used as a quality control procedure. In
    diploids, which are organisms with two copies of their genome, this
    is done through tests for Hardy-Weinberg equilibrium (HWE). However,
    for autotetraploids, which are organisms with four copies of their
    genome, the assumption of random mating and HWE are different and
    there has been less work on evaluating random mating in these
    organisms. The standard approach for HWE tests in diploids is to use
    exact tests, which control for Type I error for finite sample sizes.
    However, there are currently no exact tests available for
    autotetraploids. In this study, we provide two approaches for exact
    tests for random mating in autotetraploids. The first approach
    conditions inference on sufficient statistics, while the second uses
    a split likelihood ratio. Although these approaches exactly control
    for Type I error, simulations show that they are too conservative
    for use. Therefore, we recommend using a standard likelihood ratio
    test or a standard chi-squared test, which we implement. We
    demonstrate all of these approaches using a dataset of
    autotetraploid white sturgeon.
- Thakkar (2023): Read the thesis
  [ProQuest:2847679939](https://www.proquest.com/docview/2847679939)
  - **Abstract**: Here, we focus on testing for segregation distortion
    in F1 populations of tetraploids. Tetraploids, which contain four
    sets of chromosomes, are important in both evolutionary research and
    agricultural improvement. In agricultural experiments with F1
    populations, as a quality control measure, researchers often test
    whether genotype frequencies conform to those expected under
    Mendelian segregation. However, classical segregation patterns can
    be distorted in tetraploids due to the meiotic processes of double
    reduction and preferential pairing, which can alter gamete
    frequencies. Currently, there is no method to test for segregation
    distortion while accounting for these two processes in tetraploid F1
    populations, despite their widespread use in agriculture.

    To address this gap, we propose a Bayesian approach that
    incorporates both preferential pairing and double reduction in a new
    model for offspring genotypes in tetraploid F1 populations. We
    demonstrate the efficacy of our approach through simulations and a
    real dataset of tetraploid blueberries. Our method inherits all of
    the benefits of Bayesian analysis, including consistency under the
    null, incorporation of prior information, and applicability to small
    samples by not depending on asymptotic approximations. This study
    provides a valuable contribution to the field by offering a new tool
    for testing for segregation distortion in tetraploid F1 populations.

## Software

- The `hwep` R package: <https://cran.r-project.org/package=hwep>
  - Inference concerning equilibrium and random mating in
    autopolyploids. Methods are available to test for equilibrium and
    random mating at any even ploidy level (\>2) in the presence of
    double reduction at biallelic loci. For autopolyploid populations in
    equilibrium, methods are available to estimate the degree of double
    reduction. We also provide functions to calculate genotype
    frequencies at equilibrium, or after one or several rounds of random
    mating, given rates of double reduction. You can read about these
    methods in Gerard (2022c) and Gerard (2022a).
- The `phwelike` R package
  ([doi:10.5281/zenodo.5531955](https://doi.org/10.5281/zenodo.5531955)):
  <https://github.com/dcgerard/phwelike>
  - This package takes the methods developed and written by Jiang, Ren,
    and Wu (2021) and implements them in the form of an R package. This
    will allow researchers, such as myself, to better compare our
    methods against those of Jiang, Ren, and Wu (2021). These
    evaluations were performed in Gerard (2022c). I would recommend you
    not use this package and use the `hwep` package instead
    (<https://cran.r-project.org/package=hwep>).
- The `hexocto` R package
  ([doi:10.5281/zenodo.7019230](https://doi.org/10.5281/zenodo.7019230)):
  <https://github.com/dcgerard/hexocto>
  - This code is from Wang et al. (2021) and Wang et al. (2022), in
    package form so that it is easy to compare against other procedures.
    These evaluations are performed in Gerard (2022b). I would recommend
    you not use this package and use the `hwep` package instead
    (<https://cran.r-project.org/package=hwep>).
- The `rmexact` R package
  ([doi:10.5281/zenodo.7671765](https://doi.org/10.5281/zenodo.7671765)):
  <https://github.com/gerardlab/rmexact>
  - This package implements the exact tests for random mating in
    autotetraploids described in Matoka Nana (2023). This is joint work
    with Karene Matoka Nana.
- The `menbayes` R package
  ([doi:10.5281/zenodo.8124363](https://doi.org/10.5281/zenodo.8124363)):
  <https://github.com/gerardlab/menbayes>
  - Provides a suite of methods for Bayesian tests for Mendelian
    segregation in experimental polyploid populations (for now, just
    tetraploids). This is under different assumptions of meiosis. These
    methods are described in Thakkar (2023).

## Reproducible Research

- Results from Gerard (2022c):
  [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5531872.svg)](https://doi.org/10.5281/zenodo.5531872)
  <https://github.com/dcgerard/hwesims>
  - This code repository contains all the scripts necessary to reproduce
    the results from Gerard (2022c). We emphasize extreme reproducibilty
    by providing executable, and linked, code and data.
- Results from Gerard (2022a):
  [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6993722.svg)](https://doi.org/10.5281/zenodo.6993722)
  <https://github.com/dcgerard/rmbayes_sims>
  - This code repository reproduces all of the results from Gerard
    (2022a), including simulations and real-data analyses.
- Results from Gerard (2022b):
  [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7019205.svg)](https://doi.org/10.5281/zenodo.7019205)
  <https://github.com/dcgerard/hwesupp>
  - This code repository reproduces all of the results from Gerard
    (2022b) in the form of an interactive R markdown file.
- Results from Matoka Nana (2023):
  [![DOI](https://zenodo.org/badge/599259474.svg)](https://zenodo.org/badge/latestdoi/599259474)
  <https://github.com/gerardlab/rmexact_analysis>
  - This code repository reproduces all of the results from Matoka Nana
    (2023), including simulations and real-data analyses.
- Results from Thakkar (2023):
  [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8124372.svg)](https://doi.org/10.5281/zenodo.8124372)
  <https://github.com/gerardlab/menbayes_analysis>
  - This code repository reproduces all of the results from Thakkar
    (2023), including simulations and real-data analyses.

## Presentations

- [doi:10.5281/zenodo.5589844](https://doi.org/10.5281/zenodo.5589844):
  Slides for a presentation at the American University Department of
  Mathematics and Statistics Colloquium on 2021-10-19. This work is
  based on Gerard (2022c).

- [PAG 2022
  Poster](https://pag.confex.com/pag/xxix/meetingapp.cgi/Paper/43285):
  Virtual poster presentation at the 2022 Plant & Animal Genome
  Conference.

- [JSM 2022 Poster](https://doi.org/10.5281/zenodo.6987179): This poster
  was presented by D. Thomas Scartz at the 2022 Joint Statistical
  Meetings in Washington, DC. You can see the abstract for the poster
  [here](https://ww2.amstat.org/meetings/jsm/2022/onlineprogram/AbstractDetails.cfm?abstractid=322319).

- [PAG 2023 Poster](https://doi.org/10.5281/zenodo.7557197): PDF file of
  the poster I presented at the 2023 Plant & Animal Genome Conference.

  - Gerard, David. “Bayesian Tests for Random Mating in Autopolyploids.”
    Plant and Animal Genome Conference 30 (PAG 30), San Diego,
    California, 13–18 January 2023 (Poster PO0097).
    [DOI:10.5281/zenodo.7557197](https://doi.org/10.5281/zenodo.7557197).

- [doi:10.5281/zenodo.7893884](https://doi.org/10.5281/zenodo.7893884):
  Slides for Karene Matoka Nana’s Master’s thesis defense at American
  University on April 19, 2023. This work is based on Matoka Nana
  (2023).

- [doi:10.5281/zenodo.8190747](https://doi.org/10.5281/zenodo.8190747):
  Slides for Mira Thakkar’s Master’s thesis defense at American
  University on July 24, 2023. This work is based on Thakkar (2023).

## Education Materials

- [Advanced R Course Materials](https://dcgerard.github.io/advancedr/)
  - This course prepares students for software development using the R
    statistical programming language. Topics include: version control
    via git and its command line interface, package development, unit
    testing, base R data structures, environments, object oriented
    programming via S3 and S4, metaprogramming, interfacing with C++ via
    Rcpp, parallel processing with futures, and batch scheduling jobs
    via LSF. This course was taught during the Spring semester of 2022
    at American University. All materials that I created for this course
    are under a CC BY-NC 4.0 license, so you are free to use them for
    non-commercial purposes as long as you provide attribution.
- [Genetic Data Analysis](https://dcgerard.github.io/gda/)
  - This website contains a series of hand-written lecture notes I
    created for my research group on basic genetic data analysis. Topics
    include genotype and allele frequency estimation, Hardy-Weinberg
    equilibrium testing, linkage disequilibrium testing and estimation,
    maximum likelihood estimation and the expectation-maximization
    algorithm, basic Bayesian inference, genetic drift and mutation
    (including in the context of molecular evolution), coalescent
    theory, inbreeding, and population subdivision. I also have a few
    lectures on classic research papers. This material is under a CC
    BY-NC 4.0 license, so you can use them for non-commercial purposes
    as long as you provide attribution.

## References

<div id="refs" class="references csl-bib-body hanging-indent">

<div id="ref-gerard2022bayesian" class="csl-entry">

Gerard, David. 2022a. “Bayesian Tests for Random Mating in Polyploids.”
*bioRxiv*. <https://doi.org/10.1101/2022.08.11.503635>.

</div>

<div id="ref-gerard2022comment" class="csl-entry">

———. 2022b. “Comment on Three Papers about Hardy–Weinberg Equilibrium
Tests in Autopolyploids.” *Frontiers in Genetics* 13.
<https://doi.org/10.3389/fgene.2022.1027209>.

</div>

<div id="ref-gerard2022double" class="csl-entry">

———. 2022c. “Double Reduction Estimation and Equilibrium Tests in
Natural Autopolyploid Populations.” *Biometrics* In press.
<https://doi.org/10.1111/biom.13722>.

</div>

<div id="ref-jiang2021computational" class="csl-entry">

Jiang, Libo, Xiangyu Ren, and Rongling Wu. 2021. “Computational
Characterization of Double Reduction in Autotetraploid Natural
Populations.” *The Plant Journal* 105 (6): 1703–9.
<https://doi.org/10.1111/tpj.15126>.

</div>

<div id="ref-matokanana2023exact" class="csl-entry">

Matoka Nana, Karene. 2023. “Exact Tests for Random Mating in
Autotetraploids.” Master’s thesis, American University.
<https://doi.org/10.57912/23504199>.

</div>

<div id="ref-thakkar2023bayesian" class="csl-entry">

Thakkar, Mira. 2023. “Bayesian Tests for Segregation Distortion in
Experimental Tetraploid Populations.” Master’s thesis, American
University. <https://www.proquest.com/docview/2847679939>.

</div>

<div id="ref-wang2022asymptotic" class="csl-entry">

Wang, Jing, Li Feng, Shuaicheng Mu, Ang Dong, Jinwen Gan, Zhenying Wen,
Juan Meng, Mingyu Li, Rongling Wu, and Lidan Sun. 2022.
“<span class="nocase">Asymptotic tests for Hardy-Weinberg equilibrium in
hexaploids</span>.” *Horticulture Research* 9.
<https://doi.org/10.1093/hr/uhac104>.

</div>

<div id="ref-wang2021tracing" class="csl-entry">

Wang, Jing, Xuemin Lv, Li Feng, Ang Dong, Dan Liang, and Rongling Wu.
2021. “A Tracing Model for the Evolutionary Equilibrium of Octoploids.”
*Frontiers in Genetics* 12. <https://doi.org/10.3389/fgene.2021.794907>.

</div>

</div>
