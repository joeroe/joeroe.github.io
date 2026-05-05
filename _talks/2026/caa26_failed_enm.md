---
authors: Joe Roe
authors_short: Roe, J.
title: "Can ecological models predict the occurrence of species in the archaeological record? Can I?"
conference: "the Computer Applications and Quantitative Methods in Archaeology (CAA) annual conference, Vienna, 31 March – 4th April 2026"
date: 2026-04-03
year: 2026
month: 04
---

## Abstract

Ecological niche models, also known as species distribution models, are widely used by ecologists to quantify the relationship between the environment and the geographic extent of an organism (Sillero et al. 2021). Conceptually similar to 'predictive modelling' in archaeology, they involve training a model from known occurrences of the organism and a set of relevant environmental variables at those locations. The trained model can be studied in itself or, more commonly, used to predict the occurrence of the organism in another environmental space. This could be to anticipate the organism's response to future climate change, to model a hypothetical introduction of the organism to a new region or---most interestingly in the present context---reconstruct the palaeodistribution of the organism in a past environment. Franklin et al. (2015) observed a decade ago that the latter application could hold great interest for archaeological research – and also that data from environmental archaeology on known past occurrences could provide a key means of verifying 'hindcasted' ecological niche models. Archaeologists have (with notable exceptions) been relatively slow to take up this call, perhaps due to the difficulty of obtaining the necessary palaeoclimatic data. To my knowledge, there have been no reported uses of archaeological occurrences to verify a hindcast ecological niche model.

In a recent study (Roe and Arranz-Otaegui 2026), I used ecological niche modelling to reconstruct the terminal Pleistocene and Early Holocene biogeography of 65 plant species found regularly in association with early agricultural archaeological sites in West Asia, including the progenitors of the first crops. The scope of the study expanded significantly over the six years I worked on it, presenting technical challenges that were exacerbated by the need to incorporate a large number of 'best practices' drawn from the extensive literatures on ecological niche modelling on the one hand, and prediction using machine learning on the other. The sense of relief in finally overcoming these challenges and producing models that performed well on all the standard metrics was short-lived, however, because they all spectacularly failed to predict the real past palaeodistributions revealed by the archaeological record. When double- and triple-checking that I did the modelling correctly didn't change the situation, I was forced to invoke Box's law ("all models are wrong, but some are useful", Box 1976) and focus on other insights the results could provide.

Yet reflecting on why these models failed verification has proved, if anything, more interesting than the original study. Is it a failure of this particular model (i.e., is it just my fault)? Or is there a fundamental problem of transferability of ecological niche models applied to the past? In either case, is it possible to rectify the situation? Here I argue that, while methodological improvements could certainly be made, especially to mitigate overfitting, the mismatch between hindcast model and the archaeological record cannot simply be put down to the model being 'wrong'. Instead it prompts us to think more explicitly about what past process—or processes—these two different signals represent and, crucially, how they have been transformed. In particular, both palaeodistribution models (via the palaeoclimate surfaces used to produce them) and environmental archaeology represent temporally "mixed assemblages" (Perreault 2019, pp. 40-79), but mixed in different ways. With this in mind, the expectation that the archaeological record could straightforwardly 'verify' ecological niche models is probably too naive. But it suggests ways in which the two signals could be brought closer together, for example by formally incorporating palaeoclimatic variability and modelling of depositional processes, in a way that would benefit not just environmental archaeology but wider debates on the transferability of ecological niche models (Franklin 2023).

## References

* Box, George E P. 1976. "Science and Statistics." *J. Am. Stat. Assoc.* 71 (356): 791–99. <https://doi.org/10.1080/01621459.1976.10480949>
* Franklin, Janet. 2023. "Species Distribution Modelling Supports the Study of Past, Present and Future Biogeographies." *Journal of Biogeography* 50 (9): 1533–45. <https://doi.org/10.1111/jbi.14617>
* Franklin, Janet, Alastair J Potts, Erich C Fisher, Richard M Cowling, and Curtis W Marean. 2015. "Paleodistribution Modeling in Archaeology and Paleoanthropology." *Quat. Sci. Rev.* 110 (February): 1–14. <https://doi.org/10.1016/j.quascirev.2014.12.015>
* Perreault, Charles. 2019. *The Quality of the Archaeological Record*. Chicago: The University of Chicago Press.
* Roe, Joe, and Amaia Arranz-Otaegui. 2026. "Biogeography of Crop Progenitors and Wild Plant Resources in the Terminal Pleistocene and Early Holocene of West Asia, 14.7–8.3 ka". *Open Quaternary* 12. <https://doi.org/10.5334/oq.163>
* Sillero, Neftalí, Salvador Arenas-Castro, Urtzi Enriquez-Urzelai, Cândida Gomes Vale, Diana Sousa-Guedes, Fernando Martínez-Freiría, Raimundo Real, and A. Márcia Barbosa. 2021. "Want to Model a Species Niche? A Step-by-Step Guideline on Correlative Ecological Niche Modelling." *Ecological Modelling* 456 (September): 109671. <https://doi.org/10.1016/j.ecolmodel.2021.109671>

## Links

* [Slides](https://joeroe.io/caa26_failed_enm/)
* [Data and source code](https://doi.org/10.5281/zenodo.20035698) (Zenodo)
* [Source repository](https://github.com/joeroe/caa26_failed_enm) (GitHub)
