---
date: 2018-6-1
published: true
title: Wiki-Age Networks
description: Category and age topic modelling across wikipedia
project_tags: python, web scraping
media: project
time_period: 2018-2018
thumbnail: "/projects/wiki-age/f1.png"

website:
  button_text: Project gitlab code
  url: https://gitlab.com/thayerAlshaabi/wikiagenet

intro: |
 
 This project was conducted with excellent collabator and friend Thayer Alshaabi for a course final project in Principles of Complex Systems. See the full project write-up [here](https://sagehahn.com/images/resources/wiki-age-net.pdf)

 This project heavily features web scraping and basic NLP tools to build a dataset of information from wikipedia. Specifically, we scraped information related to notable people within fields, and and their age.
 We define at the highest level of interest, and most
 loosely, "Categories" as representative, typically, of academic disciplines. That being said, certain  Categories lend
 themselves more readily towards our proposed analysis
 such as Mathematics, Chemistry and Physics in contrast
 towards more nebulous or highly specific topics such as
 History or Geodesy. Given a Category, we next define a
 ’Branch’ as any sub topic within that larger category, say
 X, such that it would appear reasonably within a list titled
 "Branches of X" or "Fields of study of X", and importantly
 that it have an associated Wikipedia page.
 For each Category considered we sought to collect the
 following information from both its associated Wikipedia
 page and those of its Branches.

content_layout:
  - section_layout: 2col
    images:
      - caption: Branches of physics over time, where a branch is assigned a year based on the median of each person found within that branches mean year.
        description: Example 1
        url: "/projects/wiki-age/f1.png"

      - caption: Network structure for a collected branch, where node size how many people are within that category.
        description: Example 2
        url: "/projects/wiki-age/f2.png"

      - caption: Example showing the Physics branch plotting information by year and number of people.
        description: Example 3
        url: "/projects/wiki-age/f3.png"
---
