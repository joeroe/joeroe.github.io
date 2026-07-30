---
title: "era 0.6.0: chronological comparison and difference"
tag: R
---

**[era](https://era.joeroe.io)** v0.6.0 is now available [on CRAN](https://CRAN.R-project.org/package=era):

<!--more-->

```r
install.packages("era")
library(era)
```

This minor release adds functions for [chronological comparison](https://era.joeroe.io/reference/yr_earlier_than.html) of year vectors:

```r
x <- yr(c(200, 100, 300), "BCE")
yr_earlier_than(x, yr(150, "BCE"))
#> # BCE years <yr_lgl[3]>:
#> [1] FALSE FALSE  TRUE
#> # Era: Before Common Era (BCE): Gregorian years (365.2425 days), counted backwards from 1

yr_later_than(x, yr(150, "BCE"))
#> # BCE years <yr_lgl[3]>:
#> [1]  TRUE FALSE FALSE
#> # Era: Before Common Era (BCE): Gregorian years (365.2425 days), counted backwards from 1
```

And for [calculating chronological differences](https://era.joeroe.io/reference/yr_difference.html) between year vectors:

```r
yr_difference(yr(300, "BCE"), yr(100, "BCE"))
#> # years <yr[1]>:
#> [1] 200
#> # Era: Gregorian years (365.2425 days)
```

These functions are aware of era directionality: "BCE" years count backwards, so 300 BCE is earlier than 100 BCE. They support work on [tempo](https://tempo.joeroe.io), a new package I am working on that represents chronological intervals and the temporal relations between them.

## Links

* [era on CRAN](https://CRAN.R-project.org/package=era)
* [era package documentation](https://era.joeroe.io/)
* [Introductory vignette](https://era.joeroe.io/articles/era.html)
* [Source code](https://github.com/joeroe/era) (GitHub)
