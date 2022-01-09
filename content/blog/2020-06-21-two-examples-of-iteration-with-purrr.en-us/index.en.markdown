---
title: 'Two examples of iteration with purrr - Class for the RStudio certification'
author: Florencia D'Andrea
date: '2020-06-21'
slug: 'two-examples-of-iteration-with-purrr.en-us'
categories: ["Teaching"]
tags: ["teaching", "slides", "purrr", "iteration"]
subtitle: ''
summary: 'Slides created for the teaching exam of the RStudio certification'
authors: []
featured: no
header:
  image: "https://res.cloudinary.com/flor/image/upload/w_1000,ar_1:1,c_fill,g_auto,e_art:hokusai/v1592763305/14_ibvzqm.png"
  caption: ''
  focal_point: ''
  preview_only: no
projects: []
---

## RStudio Certification

I recently became certified as a RStudio Tidyverse [Instructor](https://education.rstudio.com/trainers/). To pass the certification there are two exams. In this post, I am going to share a 15 minute class that I prepared to as part of the teaching exam.


## What to teach about?

<center>

![Logo del paquete Purrr](https://res.cloudinary.com/flor/image/upload/c_scale,w_156/v1592765241/purrr_yefga4.png)

</center>

I use loops frequently for my postdoc as I need to automate tasks. That is why I decided to teach two specific examples of iteration using functions in `purrr` package.
I find that these examples are motivating for students as these functions offer a simple way to get a lot of work done:

- Read a group of files with the same extension and get a dataframe using `map_df()`

- Generate Rmarkdown reports from a list of parameters automatically with `pwalk()`

<center>

![Generate reports](https://res.cloudinary.com/flor/image/upload/v1590443438/7_eng_oi5rck.png)

</center>

## Who is the class for?

This class is part of three weeks long data analysis course for graduate students without any previous training in programming.  
The 15 minutes are part of the last class of the course. The students already have learned basic topics as visualization, data manipulation, RMarkdown, and iteration. 


## Some considerations

* To answer the the exercises in "Let's Practice" you need concepts that were explained in previous classes. Specially these 15 minutes should be teach after [iteration](https://r4ds.had.co.nz/iteration.html) and [`Rmarkdown` ](https://r4ds.had.co.nz/r-markdown.html). 

* It is not necessary to use Xaringan for the certification slides. 

* It is important that you practice your class keeping track of how long it lasts.


## Files
#### Slides
[Slides here](https://flor14.github.io/purrr_slides/purrr_class_15min#1)
<iframe src="https://flor14.github.io/purrr_slides/purrr_class_15min#1" width="672" height="300"></iframe>


#### Live coding

The file with the code for the live coding is in [Live coding.R](https://mybinder.org/v2/gh/flor14/purrr_class/e6be8080991cbd9cad0eba7b4f24858a469026a3) (wait a bit until R-Studio loads)


ðŸ±ðŸ§¶

![](https://res.cloudinary.com/flor/image/upload/v1592183718/tuna_piola_qk9jad.png)



