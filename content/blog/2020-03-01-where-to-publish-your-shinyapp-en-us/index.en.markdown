---
title: 'Where to publish your Shiny app?'
author: Florencia D'Andrea
date: '2020-03-01'
slug: where-to-publish-your-ShinyApp.en-us
categories: ["Shiny"]
tags: ["ShinyApp", "publish", "journal", "code", "software", "open source", "science"]
subtitle: ''
summary: 'My experience publishing a Shiny app - Links to lists of Scientific Journals accepting Shiny apps'
authors: []
lastmod: '2021-02-05T22:28:57-03:00'
featured: no
header:
  image: "https://res.cloudinary.com/flor/image/upload/w_1000,ar_1:1,c_fill,g_auto,e_art:hokusai/v1582548588/2_k0l388.png"
  caption: ''
  focal_point: ''
  preview_only: no
projects: []
---

## Motivation
I started to develop Shiny apps because of my research. The development of a Shiny app for the analysis of toxicological databases allowed me to explore the data in relation to different criteria.

## Where to publish?

After finishing the app, my first question was whether to publish the Shiny app. Should I include it as supplementary material of other paper or could be published as software itself?

I got valuable suggestions in the RStudio Community forum including a list of possible journals accepting Shiny apps, in the following [thread](https://community.rstudio.com/t/can-i-publish-a-shiny-app-in-a-scientific-journal-how-where/6306). I found also a lot of resources in this post: [In which journals should I publish my software? By Neil Chue Hong](https://www.software.ac.uk/which-journals-should-i-publish-my-software). Finally, I decided to try with [The Journal of Open Source Software](https://joss.theoj.org/). 

One advantage of publishing the code itself is that the journal' review process focused on how to release the code as open source software, a concept that as researchers we are barely familiarized. 

As an example, I included a file to indicate how users could contribute to my Shiny app and a license. I probably would not have done any of these steps of trying to publish the Shiny App as supplementary material of a paper.

## How good does my Shiny app have to be?

It depends on the publication venue. In my experience with JOSS, you have to make your software available in an open repository (GitHub, Bitbucket, etc.) and include an OSI approved open source license. Read more here about the other [requirements](https://joss.readthedocs.io/en/latest/submitting.html#submission-requirements).

Some considerations:

* [Make the Shiny app into an R package](https://support.rstudio.com/hc/en-us/articles/200486488-Developing-Packages-with-RStudio) 

* [Add a DOI for the Repository](https://guides.github.com/activities/citable-code/ )

* [Add version numbers](http://r-pkgs.had.co.nz/release.html)

* **Include community guidelines**. For this you can use the function `usethis::use_tidy_contributing()` 

## My first "shiny" paper

Finally, last year I published a first Shiny app to analyze ecotoxicological databases.

D’Andrea et al., (2019). [shinyssd v1.0: Species Sensitivity Distributions for Ecotoxicological Risk Assessment](https://joss.theoj.org/papers/10.21105/joss.00785). Journal of Open Source Software,
4(37), 785

## Are Scientific Papers outdated? 

I have recently read a very interesting article called [The Scientific Paper Is Outdated. By R. Abernathey](https://www.chronicle.com/article/The-Scientific-Paper-Is/248045). 

> Should scientists spend more time developing software? What do you think?

### Thanks!
I want to thank [Maëlle Salmon](https://masalmon.eu/), who encouraged me to publish this post
