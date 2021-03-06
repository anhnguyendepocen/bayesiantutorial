
---
knit: "bookdown::render_book"
title: "Bayesian Tutorial"
author: ["Devin Pastoor"]
description: "Understanding Bayesian NLME analysis"
url: 'http://www.devinpastoor.com/bayesiananalysis/'
github-repo: dpastoor/bayesiananalysis
twitter-handle: devinpastoor
site: bookdown::bookdown_site
documentclass: book
---

# Welcome {-}

This tutorial is a reasonably self-contained tutorial and documentation source about trasitioning to bayesian analysis from traditional first order estimation techniques for nonlinear-mixed-effects modeling. The overarching objective is to provide a resource for some of the additional complexity that bayesian analysis suggests/requires (mu-modeling, additional estimation tuning, etc) and to compare output under various scenarios to that of FOCE-based estimation.

As a secondary objective, this project should serve as a case study to managing a collaborative project using git, github and other 'modern' tooling for reproducible science. For contribution guidelines, see the CONTRIBUTING section below.

This work is licensed under the [Creative Commons Attribution-NonCommercial-NoDerivs 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/us/) United States License. 

# Steps

As a primary outcome of this tutorial is to understand the bayesian requirements for modeling vancomycin in 
neonates for bayesian forecasting dose recommendations, the data and parameter values will use existing
vancomycin values to get in the ballpark of outcomes to be expected from real data.

At a very high level, the following steps must be done:

* Data Generation
  * Generate covariate distributions
  * Simulate profiles for population of neonates
* Scenario 'filters'
  * sampling times
  * balance of peak/trough
  * dose modifications?
* Model fitting via FOCE
  * model building
  * covariate model building
  * proper diagnostic analyses for evaluating model adequacy/selection
* Model fitting via Bayes
  * model building
  * covariate model building
  * prior selection
  * proper diagnostic analyses for evaluating model adequacy/selection
* Model forecasting 
  * how to handle propogation of uncertainity for probability of target attainment (PTA)
  * influence of PTA output on recommendations (dose and future sampling)
