---
title: 'Sharing reproducible and interactive environments in R with Binder'
layout: single-sidebar
author: Florencia D'Andrea
date: '2020-08-28'
slug: sharing-reproducible-and-interactive-environments-in-r-with-binder.en-us
categories: ["Reproducibility"]
tags: ["Shiny", "Binder", "RStudio", "environments", "LearnR", "interactive", "LatinR", "ReproHack"]
subtitle: ''
summary: 'Shiny apps, RStudio projects and more'
lastmod: '2021-02-05T22:47:32-03:00'
featured: yes
#image:  
#  caption: '[Hi](https://res.cloudinary.com/flor/image/upload/v1598698772/github_squares_c9trzb.png)'
#  focal_point: 'Center'
#  placement: 2
#  preview_only: no
---

## Working in a reproducible manner

I'm trying to make my next paper easier to reproduce.
This has led me to read about computational reproducibility tools and get involved in communities like [ReproHack](https://twitter.com/ReproHack), where the focus is on elucidating best practices when sharing your code and data.

> Do you want to know more about ReproHack and computational reproducibility? I recommend [Anna Krystalli](https://twitter.com/annakrystalli)'s [talk on UseR! 2020](https://www.youtube.com/watch?v=KHMW8fV2NXo) 

## Binder and R?


<iframe src="https://flor14.github.io/reproducibility_slides_en/binder_reproducible_environments.html#16" width="672" height="400px" data-external="1"></iframe>

I got to know [Binder](https://mybinder.readthedocs.io/en/latest/faq.html) thanks to the [Ines Montani tutorial framework](https://github.com/ines/course-starter-r). In this framework, Binder allows you to run the code of the exercises interactively. 

One of the benefits of Binder is being able to share Shiny apps, although it has some disadvantages compared to [shinyapps.io](shinyapps.io). "Binderized" Shiny apps take longer to build but it is still an interesting alternative when leaving an application as part of a publication. It also has no restrictions on the number of apps that can be left for free. In addition, by simply changing the URL that we use to call the app, Binder allows us to access the same project using the RStudio IDE.

> If you want to deploy your Shiny app using [shinyapps.io](shinyapps.io) you can find instructions [in this webpage](https://shiny.rstudio.com/articles/shinyapps.html#:~:text=Shinyapps.io%20is%20a%20platform,such%20as%20the%20RStudio%20IDE)


A short time ago I participated in [CarpentryCon](https://carpentrycon.org/), not only helping in the [translations of lessons into Spanish](https://carpentries.org/blog/2020/08/Hablamos/), but also giving a small workshop with Pablo Bernabeu on Reproducibility and Open Science where I briefly explained the use of Binder for R users.

If you want to know more about Binder, I suggest [The Turing Way book](https://the-turing-way.netlify.app/welcome). The [Turing Way](https://twitter.com/turingway) is another community that I recommend you follow if you are interested in the topic of open science and reproducibility.

> Tutorials: Binder is part of the Inés Montani framework for R and Python tutorials and can also be used to share [learnR tutorials as it is explained in this blog post](https://syoh.org/learnr-tutorial/)


## Slides

<center>

![](https://res.cloudinary.com/flor/image/upload/c_scale,w_460/v1599145015/charlaR_con_R_3_paoy3a.png)

</center>

I prepared these [slides](https://flor14.github.io/reproducibility_slides_en/binder_reproducible_environments.html#1) as part of a meetup to present the first ReproHack in Spanish to be held at the [LatinR](https://latin-r.com/en) 2020 conference.

In these slides you can find:

* Different ways to capture computational environments 

* A brief overview of the `renv` package

* What Binder is

* Steps to share interactive environments with Binder.


<iframe src="https://flor14.github.io/reproducibility_slides_en/binder_reproducible_environments.html#21" width="672" height="400px" data-external="1"></iframe>

Slides in [English](https://flor14.github.io/reproducibility_slides_en/binder_reproducible_environments.html#1).

Slides in [Spanish](https://flor14.github.io/r_de_reproducibilidad/r_de_reproducibilidad.html#1).

# Final note

Due to [changes to Docker terms of service](https://www.docker.com/blog/scaling-docker-to-serve-millions-more-developers-network-egress/) on November 1st the lack of activity for 6 months may cause the sharing link to become inactive.
You can ask questions about Binder in the following link https://discourse.jupyter.org/

