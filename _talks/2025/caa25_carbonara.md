---
authors: Martin Hinz and Joe Roe
authors_short: Hinz, M. & Roe, J.
title: "Open-Source Bayesian Chronological Modeling: The Role of a Domain-Specific Language"
conference: "the Computer Applications and Quantitative Methods in Archaeology (CAA) annual conference, Athens, 5–9 May 2025"
date: 2025-05-06
year: 2025
month: 5
---

## Abstract

Radiocarbon (^14C) dating is a fundamental tool in archaeology and related disciplines for establishing chronological frameworks. Calibration of radiocarbon dates is essential to account for fluctuations in atmospheric ^14C over time, and Bayesian statistical methods have become increasingly important for refining these calibrations with additional information. For decades, OxCal has been the dominant software for radiocarbon calibration, particularly renowned for its ability to integrate stratigraphic and prior information through its domain-specific language (DSL) [1]. OxCal’s DSL allows users to construct complex chronological models that incorporate sequences, phases, and other stratigraphic relationships, making it indispensable for many researchers.

While other calibration software exists — such as BCal [2], CalPal [3], ChronoModel [4], and the R packages ‘rcarbon’ [5] and ‘Bchron’ [6] — these tools have not yet fully replicated OxCal’s capacity to merge stratigraphic information with dating results in a comprehensive Bayesian framework. This limitation restricts the ability of researchers to construct detailed chronological models within a single, open-source environment.

Our own tool, ‘OxcAAR’ [7], has been developed as an interface between R and OxCal, allowing users to access OxCal’s functionalities directly from R scripts. OxcAAR translates elements of OxCal’s DSL into R commands, enabling some degree of integration and automation within the R environment. However, it remains dependent on OxCal as the underlying engine, which poses challenges related to software dependency, licensing, and extensibility.

The ultimate goal is to develop a fully open-source alternative to OxCal that matches or surpasses its functionality, particularly in terms of integrating stratigraphic information and radiocarbon dating within a Bayesian framework. This endeavor raises critical questions about the approach to adopting or adapting a DSL for the new software. Should we continue with OxCal’s existing DSL to maintain familiarity and ease the transition for users, or should we develop a new DSL that could offer improved functionality and integration with modern programming languages?

Continuing with OxCal’s DSL presents both opportunities and obstacles. On one hand, it could facilitate adoption by allowing users to apply their existing knowledge and potentially port their models with minimal adjustments. On the other hand, OxCal’s DSL may have limitations that are not easily adapted to an open-source context or may not align well with the syntax and paradigms of languages like R or Python. Furthermore, replicating the DSL in a new software could raise concerns about intellectual property and might limit the potential for innovation in the modeling language.

Alternatively, developing a new DSL tailored to the open-source environment offers the possibility of creating a language that integrates seamlessly with modern programming practices, enhances usability, and allows for greater extensibility. However, this approach comes with the challenge of requiring users to learn a new language, which could hinder adoption. It also necessitates careful design to ensure that the new DSL is capable of expressing the complex chronological models that researchers require.

In our efforts to create an open-source alternative, we are aiming for practically addressing these questions through the development of a new R package. This package shall provide the functionalities of OxCal within the R environment, leveraging R’s powerful statistical and programming capabilities. We are exploring the design of a DSL that is both expressive and user-friendly, allowing researchers to define complex chronological models while taking advantage of R’s syntax and structures.

One approach under consideration is to create a DSL that borrows concepts from OxCal but is adapted to fit naturally within R’s programming paradigm. This could involve using R functions and syntax to represent sequences, phases, and stratigraphic relationships, thereby providing a familiar yet flexible interface for users. By integrating the DSL within R, we aim to enhance reproducibility, facilitate integration with other analytical workflows, and promote open science practices.

As we progress, we are mindful of the need to balance the advantages of familiarity with the benefits of innovation. We would like to engage with the research community to gather feedback on aspects of usability, required features, and potential barriers to adoption. Lessons learned from the implementation of OxcAAR suggest that it is feasible to replicate key functionalities of OxCal within an open-source framework, though further work is needed to fully realize this potential.

In this presentation, we will discuss the conceptual framework of our initiative, the considerations involved in choosing or designing a DSL for chronological modeling, and the practical steps that need to be taken to develop such a software. We will highlight the capabilities of existing calibration software, and how our approach seeks to complement and extend these tools by incorporating stratigraphic information in a Bayesian context.

By sharing our experiences and the challenges, we aim to contribute to the broader discussion on advancing open-source tools in radiocarbon calibration and chronological modeling. Our goal is to foster collaboration and invite input from the community to develop a tool that meets the evolving needs of researchers in archaeology and related fields.

## References

1. Bronk Ramsey, C. (2009). Bayesian analysis of radiocarbon dates. Radiocarbon, 51(1), 337–360. doi:10.1017/S0033822200033865
2. Buck C.E., Christen J.A. and James G.N. (1999). BCal: an on- line Bayesian radiocarbon calibration tool. Internet Archaeology, 7. (http://intarch.ac.uk/journal/issue7/buck/).
3. Bernie Weninger. (2024). CalPal Edition 2024.11. Zenodo. https://doi.org/10.5281/zenodo.14197386
4. ChronoModel Development Team. (2015). ChronoModel: Chronological modelling of archaeological data using Bayesian statistics. Available at: https://chronomodel.com
5. Crema, E. R., Bevan, A., & Shennan, S. (2017). rcarbon: Calibration and analysis of radiocarbon dates. R Package Version 1.4.2. Available at: https://cran.r-project.org/package=rcarbon
6. Haslett, J., & Parnell, A. (2008). A simple monotone process with application to radiocarbon-dated depth chronologies. Journal of the Royal Statistical Society: Series C (Applied Statistics), 57(4), 399–418.
7. Hinz, M., Schmid, C., Knitter, D., & Tietze, C. (2018). OxcAAR: Interface from R to OxCal. Journal of Open Source Software, 3(22), 640. doi:10.21105/joss.00640

## Links

* [Presentation source code and data](https://github.com/MartinHinz/caa2025_dsl_presentation) (GitHub)
* [Carbonara Proof of Concept](https://github.com/MartinHinz/carbonara_poc) (GitHub)
