---
date: 2022-5-1
published: true
title: "Brain Predictability Toolbox"
description: "The Brain Predictability toolbox (BPt), is a python based Machine Learning library designed for neuroimaging."
project_tags: python, ML, NeuroImaging
media: Website
ownership:
time_period: 2020-present
thumbnail: "/projects/bpt/red_logo.jpg"

website:
  button_text: Visit the project documentation
  url: https://sahahn.github.io/BPt/

intro: |
  The Brain Predictability toolbox (BPt) represents a unified framework of machine learning (ML) tools designed to work with both tabulated data (e.g. brain derived, psychiatric, behavioral and physiological variables) and neuroimaging specific data (e.g. brain volumes and surfaces). This package is suitable for investigating a wide range of different neuroimaging-based ML questions, in particular, those queried from large human datasets.

  The project source code is hosted through [github](https://github.com/sahahn/BPt), as well as the project [documentation](https://sahahn.github.io/BPt/). A paper describing this work  was published in [Bioinformatics](https://academic.oup.com/bioinformatics/article-abstract/37/11/1637/5995310?login=false) in 2021, and is also avaliable on [arvix](https://arxiv.org/abs/2011.01715).

  This project represents the largest and most consistent of any project I have worked on. In the process of developing the library, I learned a great deal about how to generally structure growing code-bases as well as what not to do... (the first iteration of the project may or may not have grown into a giant god class that I had to spend two weeks de-fusing into its current state). The current version of the library has all sorts of other nice things built in too, like automatically generated documentation, CI testing across devices through GitHub Actions and more.


content_layout:

  - section_layout: 2col
    images:
      - caption: Screenshot from github
        description: 'Github'
        url: '/projects/bpt/bpt2.png'

      - caption: Example of loading data into Dataset object
        description: 'Example  1'
        url: '/projects/bpt/bpt4.png'

      - caption: Screenshot from documentation
        description: 'Docs'
        url: '/projects/bpt/bpt1.png'
        
      - caption: Example of running default ML Pipeline
        description: 'Example 2'
        url: '/projects/bpt/bpt3.png'

---
