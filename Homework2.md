Homework 2
================

### Experiment Protocol Analysis

**Possible Protocols**

*PP1*  
Roll die once, if \(X = 6\), then conclude the die is unfair. If
\(X = 1, 2, 3, 4, 5\), then conclude the die is fair.

With such a small sample, the probability that we would determine what
is actually a fair die to be unfair is \(1/6\). Conversely, if the die
were unfair, the probability that we would deem it to be fair is ( \<
5/6). Given that the unfair die is weighted to roll a 6 more than 1/6
times, the numbers 1 to 5 would be rolled less than 5/6 times. Depending
on the weightedness of the die, that probability could even be zero.

*PP2*  
Roll die 30 times.

Decision Rule: The expected number of outcomes where (x = 6) is the
probability of rolling a 6 times the number of trials. 1/6 \* 30 = 5. If
we observe 6 approximately 5 times, we can conclude that the die is
fair.

Were we to roll a fair die, we would expect to observe a 6 on 5
occasions. We can approach the problem using a binomial distribution -
we either observe a 6, classified as a success, or we do not observe a
6, a failure. We would expect to roll a 6 on 5 occasions 19.2% of the
time. Rolling one more or one less 6 would occur 16% and 18.5% of the
time, respectively.

Our sample size and probability of success is large enough to let us
approximate the binomial using the normal distribution. Accounting for
the continuity correction, the probability of rolling a 6 on 4 or 6
occasions is 17.2%, each. Rolling a 6 from 4 to 6 times would occur
37.6% of the time. I conclude that it is not particularly unusual to
roll one more or one less 6.

Below is a table of probabilities from the binomial distribution:

``` r
read.csv("PP2outcomes.csv", fill = FALSE, nrow = 8)
```

    ##   X...6 Probability  X X.1 X.2 X.3 X.4 X.5 X.6 X.7 X.8 X.9
    ## 1     2      0.0732 NA  NA  NA  NA  NA  NA  NA  NA  NA  NA
    ## 2     3      0.1368 NA  NA  NA  NA  NA  NA  NA  NA  NA  NA
    ## 3     4      0.1847 NA  NA  NA  NA  NA  NA  NA  NA  NA  NA
    ## 4     5      0.1921 NA  NA  NA  NA  NA  NA  NA  NA  NA  NA
    ## 5     6      0.1601 NA  NA  NA  NA  NA  NA  NA  NA  NA  NA
    ## 6     7      0.1098 NA  NA  NA  NA  NA  NA  NA  NA  NA  NA
    ## 7     8      0.0632 NA  NA  NA  NA  NA  NA  NA  NA  NA  NA
    ## 8    NA          NA NA  NA  NA  NA  NA  NA  NA  NA  NA  NA

As with one more or less, rolling a 6 on 2 more or 2 less occasions sits
within 1 standard deviation of the mean, so it is not particularly
unusual. We would expect approximately 68% of our samples to produce a 6
on 3, 4, 5, 6 or 7 occasions. Rolling a 6 three more or less times is
less common - a 6 occurring twice or 8 times are approximately 1.47
standard deviations from the mean of 5.

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
