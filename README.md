# pwrAB

**pwrAB** is a simple package to perform power analysis for AB testing. There are a number of R packages for power calculations, such as the widely used **pwr** package, but to my knowledge none of the t-test power functions allow the variance and sample size to simultaneously vary across the two groups. Instead, they are based on the pooled t-test, and will provide biased results when the variance and sample size are not equal across groups.

The two functions in the pwrAB package use the Welch's unequal variance t-test instead, and will provide valid results even when sample sizes are unequal. [Delacre et al. (2017)](http://www.rips-irsp.com/articles/10.5334/irsp.82/) expands on this topic in more detail for those that are interested.

The package is [available on CRAN](https://cran.r-project.org/web/packages/pwrAB/index.html), and can be easily installed by typing:
```
install.packages('pwrAB')
```

Much of the code/syntax of this package is borrowed from the [**pwr** package by Champely et al.](https://cran.r-project.org/web/packages/pwr/index.html). Many thanks to the authors for making their code publicly available.
