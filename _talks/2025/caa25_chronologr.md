---
authors: Gilles Geeraerts, Joe Roe, and Eythan Levy
authors_short: Geeraerts, G., Roe, J., & Levy, E.
title: "A command-line interface for chronological network modelling in R"
conference: "the Computer Applications and Quantitative Methods in Archaeology (CAA) annual conference, Athens, 5–9 May 2025"
date: 2025-05-06
year: 2025
month: 5
---

## Abstract

Chronological networks (Levy et al. 2021) are a robust new approach to formally modelling complex chronologies drawn from archaeological and historic data.
The method has been implemented in the software *[ChronoLog](https://chrono.ulb.be/)*, which provides a graphical user interface for interactively building and evaluating chronological network models.
Here we introduce a new implementation of chronological networks in the R statistical programming language.
The *chronologr* package ports the *ChronoLog*'s chronological network data structure and core algorithms from Java to R.
These include the functionality to translate user-provided temporal contraints and relations to a graph format, check its logical consistency, and (if consistent) 'tighten' it to give the narrowest possible temporal constraints (i.e. date ranges) on the chronology.
Since we had an existing reference implementation in Java, and most of the underlying graph algorithms needed to implement these functions are available in R through the *igraph* library (Csardi and Nepusz 006), this part of the implementation is relatively straightforward.

A more challenging aspect of bringing chronological networks to R was adapting *ChronoLog*'s graphical interface to a scripted command line.
This required us to rethink the UI patterns used for data import, model construction, and querying of the output, as those that worked well in a graphical environment did not naturally translate to a scripted one.
We also faced the challenge of translating *ChronoLog*'s underlying object-oriented application programming interface (API) to better fit R's functional idiom.

In particular, a major strength of the *ChronoLog* GUI is that it facilitates iterative model building by giving the user instant feedback on how changes to the network and temporal constraints affect the 'tightened' chronology.
Bringing this to the R interface was one of our key aims, which we approached by implementing a simple domain-specific language (DSL) for building chronological network models.
This consists of a set of declarative functions by which users can progressively construct a model, as an alternative to simply providing its specification as input data.
In this way, the R script itself serves as a human–readable description of the model, allowing for easier reproduction and, crucially, for the user to iteratively adjust the model in response to feedback from the consistency check and tightening procedures.
The syntax of these functions are closely modelled on existing 'tidy'-style DSLs in *ggplot2* and other popular R packages (Wickham 2014, ch. 15), which provides a familiar interface for a large number of R users and facilitates the integration of *chronologr* into data analysis pipelines using other packages.

## References

* Csardi, Gabor, and Tamas Nepusz. 2006. "The Igraph Software Package for Complex Network Research." *InterJournal Complex Systems*: 1695. <https://igraph.org>.
* Levy, Eythan, Gilles Geeraerts, Frédéric Pluquet, Eli Piasetzky, and Alexander Fantalkin. 2021. "Chronological Networks in Archaeology: A Formalised Scheme." *Journal of Archaeological Science* 127 (March): 105225. <https://doi.org/10.1016/j.jas.2020.105225>.
* Wickham, Hadley. 2014. *Advanced R*. 1st edition. The R Series. CRC Press.

## Links

* [chronologr source code](https://github.com/joeroe/chronologr) (GitHub)
