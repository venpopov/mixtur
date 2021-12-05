
<!-- README.md is generated from README.Rmd. Please edit that file -->

[![](http://www.r-pkg.org/badges/version/mixtur)](https://cran.r-project.org/web/packages/mixtur/index.html)
[![](http://cranlogs.r-pkg.org/badges/grand-total/mixtur)](https://cran.r-project.org/web/packages/mixtur/index.html)

# mixtur <a ><img src='images/logo/mixtur_logo.png' align="right" height="250" /></a>

**mixtur** is an R package for designing, analysing, and modelling
continuous report visual short-term memory studies. The package allows
users to implement the 2-component (Zhang & Luck, 2008) and 3-component
(Bays, Catalao, & Husain, 2009) mixture models of continuous-report
visual short-term memory data. The package can also fit & simulate the
slots and slots-plus averaging models of Zhang & Luck.

The package allows users to:

  - Obtain summary statistics of response error and response precision
    of behavioural data
  - Produce publication-ready plots of behavioural data
  - Fit both the 2- and 3-component models to user data
  - Plot the goodness of model fit to user data
  - Simulate artificial data from both models
  - Conduct formal model competition analysis

## Installation

You can install the released version of mixtur (v1.2.0) from
[CRAN](https://cran.r-project.org/web/packages/mixtur/index.html) with:

``` r
install.packages("mixtur")
```

The development version (v1.2.0.9000) can be installed from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("JimGrange/mixtur")
```

## Pre-print

We have a paper showing users how to use the package. A pre-print of the
paper can be found here:

  - Grange, J.A. & Moore, S.B. (in press). mixtur: An R package for
    designing, analysing, and modelling continuous report visual
    short-term memory studies. *Behavior Research Methods.*
    <https://psyarxiv.com/n6gqx/>

The pre-print also includes several simulation studies exploring some
properties of the models (including parameter recovery simulations,
model recovery simulations) and provide concrete recommendations to
researchers wishing to use mixture modelling in their own research.

## Acknowledgements & References

  - We are grateful to Ed. D.J. Berry who contributed to the package
    development.

  - Portions of the package code have been adapted from code written by
    Paul Bays in Matlab, with permission. We are extremely grateful to
    Paul Bays for this permission. See <https://paulbays.com>.

  - Bays, P. M., Catalao, R. F. G., & Husain, M. (2009). The precision
    of visual working memory is set by allocation of a shared resource.
    *Journal of Vision, 9*(10): 7, 1–11.

  - Zhang, W., & Luck, S. J. (2008). Discrete fixed-resolution
    representations in visual working memory. *Nature, 453,* 233–235.
