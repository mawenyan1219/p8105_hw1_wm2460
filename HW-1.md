HW 1
================

## Question 1

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

The means flipper length is 200.9152.

#### Scatterplot

When you click the **Knit** button a document will be generated that
includes both content as well as the output of any embedded R code
chunks within the document. You can embed an R code chunk like this:

``` r
summary(cars)
```

    ##      speed           dist       
    ##  Min.   : 4.0   Min.   :  2.00  
    ##  1st Qu.:12.0   1st Qu.: 26.00  
    ##  Median :15.0   Median : 36.00  
    ##  Mean   :15.4   Mean   : 42.98  
    ##  3rd Qu.:19.0   3rd Qu.: 56.00  
    ##  Max.   :25.0   Max.   :120.00

## Including Plots

You can also embed plots, for example:

![](HW-1_files/figure-gfm/pressure-1.png)<!-- -->

Note that the `echo = FALSE` parameter was added to the code chunk to
prevent printing of the R code that generated the plot.
