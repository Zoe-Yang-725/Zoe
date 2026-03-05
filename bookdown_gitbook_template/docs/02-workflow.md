# Workflow

## Typical analysis workflow

1. Data import
2. Data cleaning
3. Exploratory Data Analysis (EDA)
4. Modelling
5. Reporting

## Example: simple plot


``` r
set.seed(123)
y <- cumsum(rnorm(200))
plot(y, type = "l", main = "Example time series", xlab = "t", ylab = "value")
```

<img src="02-workflow_files/figure-html/unnamed-chunk-1-1.png" alt="" width="672" />
