HW 1
================

## Problem 1

#### Description of “penguins” dataset

The name of the penguins dataset are species, island, bill_length_mm,
bill_depth_mm, flipper_length_mm, body_mass_g, sex, year. This data set
contains physical traits information about the different species of
penguins in some islands.

There are 344 observations and 8 variables in this dataset.

``` r
mean(penguins$flipper_length_mm,na.rm = TRUE)
```

    ## [1] 200.9152

The means flipper length is
`mean(pull(.penguins, var = flipper_length_mm))`

The means flipper length is 200.9152047

#### Scatterplot

``` r
penguins_plot_df = tibble(
  x = penguins$bill_length_mm,
  y = penguins$flipper_length_mm,
  Species = penguins$species
)

ggplot(penguins_plot_df, aes(x = x, y = y, color = Species)) + geom_point()
```

    ## Warning: Removed 2 rows containing missing values (geom_point).

![](HW-1_files/figure-gfm/scatterplot_penguins-1.png)<!-- -->

ggsave(“penguins_plot.pdf”, height = 4, width = 6)

## Problem 2

``` r
p2_df = tibble(
  norm_samp = rnorm(10),
  norm_samp_pos = norm_samp > 0,
  
)

samp = rnorm(100)
length(samp)
```

    ## [1] 100

la_df = tibble( norm_samp = rnorm(500, mean = 1), norm_samp_pos =
norm_samp \> 0, abs_norm_samp = abs(norm_samp) )
