---
title: "controller: tidy messy terminology in R with controlled vocabularies"
tag: R
---

[controller](https://controller.joeroe.io) is an R package for working with controlled vocabularies. 
It's first release (v0.1.0) is now available now [on CRAN](https://cran.r-project.org/package=controller).

The package addresses something I find myself doing very often in analysis code: tidying messy and inconsistent terminologies.
For smaller datasets, `dplyr::recode()` is okay for this, but writing the mapping out as an R function call gets tedious fast when dealing with a long list of terms.
It becomes *very* tedious when you have variants distinguished only by things like capitalisation (`OxA-` vs. `oxa-`), word boundaries (`Çatalhöyük` vs. `Çatal Höyük`) or character encoding (`ʿAin Ghazal` vs. `ʽAyn Ghazal`).

controller instead defines preferred terms and their variants in a data frame.
Its `control()` verb is the equivalent of `dplyr::recode()` but using this thesaurus and with a few extra bells and whistles for fuzzy matching and reporting what was (and wasn't) changed:

```r
library(controller)
data("colour_thesaurus")

shades <- c("daffodil", "purple", "magenta", "azure", "navy", "violet")
control(shades, colour_thesaurus)
#> Replaced values:
#> ℹ daffodil → yellow
#> ℹ azure → blue
#> ℹ navy → blue
#> ℹ violet → purple
#> Warning: Some values of `x` were not matched in `thesaurus`:
#> ✖ magenta
```

Fuzzy matching means we don't need to exhaustively list those variants from things like differences in case, word boundaries, or character encoding:

```r
control_ci(toupper(shades), colour_thesaurus)
#> Replaced values:
#> ℹ DAFFODIL → yellow
#> ℹ PURPLE → purple
#> ℹ AZURE → blue
#> ℹ NAVY → blue
#> ℹ VIOLET → purple
#> [1] "yellow"  "purple"  "MAGENTA" "blue"    "blue"    "purple"
#> Warning message:
#> Some values of `x` were not matched in `thesaurus`:
#> ✖ MAGENTA
```

---

This package has been hanging around for a while!
It started off as a helper function I used for cleaning up site names from prehistoric sites in Southwest Asia.
The basic idea was inspired by similar functions that used to exist in [c14bazAAR](https://github.com/ISAAKiel/c14bazAAR) for cleaning sample metadata for radiocarbon date, that I thought were quite neat.
So when the maintainers of that package decided to deprecate those, I took over the thesauri as part of [c14](https://c14.joeroe.io) and spun the supporting functions off into controller as a standalone package.
Then over the years it acquired some more functionality for working with controlled vocabularies (a surprising gap in the R ecosystem), like reading heritage vocabularies in [Historic England's FISH format](https://heritage-standards.org.uk/fish-vocabularies/).
Five years later, I am finally getting around to releasing it on CRAN because I need to release c14 on CRAN, because *that's* used in analyses I'm now publishing.
It's the research software engineering of [changing a lightbulb](https://www.youtube.com/watch?v=5W4NFcamRhM), basically.

---

The first release of controller includes:

- `control()`, `control_ci()`, and `control_fuzzy()` for recoding values
- `control_names()`, `control_names_ci()`, and `control_names_fuzzy()` for recoding names
- `control_matches()` for inspecting how matches were made
- `read_fish()` for reading vocabularies in [Historic England's FISH format](https://heritage-standards.org.uk/fish-vocabularies/)
- `colour_thesaurus`, an example dataset

You can install it from CRAN:

```r
install.packages("controller")
```

Or the development version from GitHub:

```r
remotes::install_github("joeroe/controller")
```

You can find the full documentation at <https://controller.joeroe.io>.
