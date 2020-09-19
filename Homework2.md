Homework 2
================

### Experiment Protocol Analysis

**Possible Protocols**

*PP1*  
Roll die once, if \(X = 6\), then conclude the die is unfair. If
\(X != 6\), then conclude the die is fair.

With such a small sample, the probability that we would determine what
is actually a fair die to be unfair is \(1/6\). Conversely, if the die
were unfair, the probability that we would deem it to be fair is $ \<
5/6$. Given that the unfair die is weighted to roll a 6 more than 1/6
times, the numbers 1-5 would be rolled less than 5/6 times. Depending on
the weightedness of the die, that probability could even be zero.

## Including Code

You can include R code in the document as follows:

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

![](Homework2_files/figure-gfm/pressure-1.png)<!-- -->

Note that the `echo = FALSE` parameter was added to the code chunk to
prevent printing of the R code that generated the plot.
