
# mixtur: An R package for designing, analysing, and modelling continuous report visual short-term memory studies

**mixtur** is a package to assist researchers in designing, analysing,
and modelling data from continuous report visual short-term memory
studies.

## Installation

To install the package from GitHub, you need the devools package:

``` r
install.packages("devtools")
library(devtools)
```

Then **mixtur** can be directly installed:

``` r
devtools::install_github("JimGrange/mixtur")
```

## Continuous Report Tasks

![](images/overview.png)

In continuous report tasks, participants are presented with an encoding
screen with items to remember (in this example, the participants need to
recall the colours of the squares). After a retention interval, one of
the squares is probed (highlighted here by the darkened square), and the
participants’ task is to recall the colour of the probed item.

The participant makes their response on a colour wheel, and the
dependent variable is the angular deviation between the participant’s
response (R) and the true target value (T) in radians.

After many trials, a probability density distribution can be formed of
the response errors across participants.

## Example Data

**mixtur** includes several example data sets to allow the user to
familiarise themselves with the package:

  - **bays2009\_full**: The full data set from Bays et al. (2009)
    including set size manipulations (1, 2, 4, and 6 items) plus a
    manipulation of *delay* of the retention interval (100ms, 500ms, and
    2,000ms).
  - **bays2009\_sample**: A sample from Bays et al. (2009).

Data can be loaded in the following way:

``` r
library(mixtur)
#> Loading required package: tidyverse
#> ── Attaching packages ─────────────────────────────────────────────── tidyverse 1.3.0 ──
#> ✓ ggplot2 3.3.2     ✓ purrr   0.3.4
#> ✓ tibble  3.0.3     ✓ dplyr   1.0.0
#> ✓ tidyr   1.1.0     ✓ stringr 1.4.0
#> ✓ readr   1.3.1     ✓ forcats 0.5.0
#> ── Conflicts ────────────────────────────────────────────────── tidyverse_conflicts() ──
#> x dplyr::filter() masks stats::filter()
#> x dplyr::lag()    masks stats::lag()
#> Loading required package: RColorBrewer
data(bays2009_sample)
head(bays2009_sample)
#>   id response target non_target_1 non_target_2 non_target_3
#> 1  1   -2.186 -0.002       -2.989        2.648        2.262
#> 2  1   -1.980 -2.498       -1.861       -1.340       -0.309
#> 3  1   -0.177 -2.088       -2.845       -3.102       -0.371
#> 4  1    1.342  1.334        2.844        1.007       -0.599
#> 5  1   -1.644 -2.224        3.129        2.936        1.295
#> 6  1    1.219  1.253        2.886       -0.924       -1.035
```

## References
