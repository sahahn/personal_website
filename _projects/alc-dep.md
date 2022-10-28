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
  button_text: Visit the project github
  url: https://github.com/sahahn/Alc_Dep

intro: |
  This work was published in the journal of Human Brain Mapping in October of 2020, and can be found [here](https://onlinelibrary.wiley.com/doi/full/10.1002/hbm.25248).
  
  This project was to identify neuroimaging biomarkers of alcohol dependence (AD) from structural magnetic resonance imaging. Data were grouped into a training set used for internal validation including 1,652 participants (692 AD, 24 sites), and a test set used for external validation with 382 participants (146 AD, 3 sites).

  This project included an exploratory data analysis, followed by a novel evolutionary search based feature selection procedure, designed to select to
  highest performing and more generalizable subset of brain measurements. 

content_layout:

  - section_layout: 2col
    images:

      - caption: This project sourced a quite varied collection of data from different sites, with very different underlying distributions of case to control.
        description: 'Data distrubtion'
        url: '/projects/alc-dep/alc2.jpg'

      - caption: a. The top 15 features (threshold chosen for readability), as ranked by average weighted feature importance (where 0 indicates a  feature appeared in none of the GA final models, and 1 represents a feature appeared in all) are shown. b. The cortical thickness and b. cortical average surface area feature importance scores, above an a priori selected threshold of 0.1, are shown as projected onto the fsaverage surface space.
        description: 'Results'
        url: '/projects/alc-dep/alc.jpg'

---
