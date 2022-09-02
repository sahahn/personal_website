---
date: 2019-1-1
published: true
title: "Predicting Alcohol Dependence"
description: "A research project investigating prediction of alcohol dependence from multi-site brain structural measures."
project_tags: python, ML, NeuroImaging
media: Research Paper
ownership:
time_period: 2019-2020
thumbnail: "/projects/alc-dep/alc.jpg"

website:
  button_text: Github
  url: https://github.com/sahahn/Alc_Dep

intro: |
  This work was published in the journal of Human Brain Mapping in October of 2020, and can be found [here](https://onlinelibrary.wiley.com/doi/full/10.1002/hbm.25248).

  To identify neuroimaging biomarkers of alcohol dependence (AD) from structural magnetic resonance imaging, it may be useful to develop classification models that are explicitly generalizable to unseen sites and populations. This problem was explored in a mega-analysis of previously published datasets from 2,034 AD and comparison participants spanning 27 sites curated by the ENIGMA Addiction Working Group. Data were grouped into a training set used for internal validation including 1,652 participants (692 AD, 24 sites), and a test set used for external validation with 382 participants (146 AD, 3 sites). An exploratory data analysis was first conducted, followed by an evolutionary search based feature selection to site generalizable and high performing subsets of brain measurements. Exploratory data analysis revealed that inclusion of case- and control-only sites led to the inadvertent learning of site-effects. Cross validation methods that do not properly account for site can drastically overestimate results. Evolutionary-based feature selection leveraging leave-one-site-out cross-validation, to combat unintentional learning, identified cortical thickness in the left superior frontal gyrus and right lateral orbitofrontal cortex, cortical surface area in the right transverse temporal gyrus, and left putamen volume as final features. Ridge regression restricted to these features yielded a test-set area under the receiver operating characteristic curve of 0.768. These findings evaluate strategies for handling multi-site data with varied underlying class distributions and identify potential biomarkers for individuals with current AD.

content_layout:

  - section_layout: 2col
    images:
      - caption: a. The top 15 features (threshold chosen for readability), as ranked by average weighted feature importance (where 0 indicates a  feature appeared in none of the GA final models, and 1 represents a feature appeared in all) are shown. b. The cortical thickness and b. cortical average surface area feature importance scores, above an a priori selected threshold of 0.1, are shown as projected onto the fsaverage surface space.
        description: 'Results'
        url: '/projects/alc-dep/alc.jpg'

      - caption: This project sourced a quite varied collection of data from different sites, with very different underlying distributions of case to control.
        description: 'Data distrubtion'
        url: '/projects/alc-dep/alc2.jpg'

---
