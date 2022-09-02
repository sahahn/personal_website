---
date: 2020-1-3
published: true
title: "Evolutionary Generated Parcellations"
description: "Evolutionary generated task fMRI surface parcellations."
project_tags: python, NeuroImaging, Research
media: Website
ownership:
time_period: 2020-2020
thumbnail: "/projects/parcel-search/generate.gif"

website:
  button_text: Visit the project github.
  url: https://github.com/sahahn/Parcel_Search

intro: |
    This project, while ultimately unsuccesful, aimed to generate novel parcellations based on their predictive merit. To do this,
    a specially designed evolutionary search was performed, where parcellations themselves were mutated and evaluated.
    The project source code is hosted through [github](https://github.com/sahahn/Parcel_Search).

    A slide deck containing a detailed description of the project, as well as results + interpretation can be found [here](https://docs.google.com/presentation/d/15acie-MotSbmBgjtz1Cy2Ra6R32l-b0qKq68x8Cl4r4/edit?usp=sharing).

    The eventual key take-away from this work was actually the realization that parcellations with higher numbers of parcels performed better than their lower
    parcel counter-parts. This led to follow-up work in [Performance Scaling for Parcellations](../parc-scaling)


content_layout:

  - section_layout: 2col
    images:
      - caption: Visualizing how random parcellations were generated from a series of seed regions in this project.
        description: Generate a new random parcellation.
        url: '/projects/parcel-search/rand_parc.gif'
    videos:
      - caption: Process outlining a simple example of how parcellations were generated and evaluated in the context of the evolutionary search.
        description: Github
        url: 'https://www.youtube.com/embed/fAOiT886qB8'

---

