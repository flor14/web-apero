---
title: 'Recipe for your first interactive tutorial'
author: Florencia D'Andrea
date: '2020-03-28'
slug: cooking-your-first-tutorial.en-us
categories: ["Tutorials"]
tags: ["Tutorials", "Ines Montani", "Framework"]
subtitle: ''
summary: 'An initial guide on how to start an interactive tutorial from scratch using Ines Montani framework'
authors: []
lastmod: '2021-02-05T22:38:53-03:00'
featured: no
header:
  image: "https://res.cloudinary.com/flor/image/upload/w_1000,ar_1:1,c_fill,g_auto,e_art:hokusai/v1584660577/3_zru9mg.png"
  caption: ''
  focal_point: ''
  preview_only: no
projects: []
---
May 2020: Interview available on the RStudio blog about the tutorials https://education.rstudio.com/blog/2020/05/teach-interactive-course/

> The aim of this post is to provide a route map highlighting the resources available to generate your own tutorial.

## Hello

Last year I helped to transform some courses from a DataCamp format to Ines Montani framework. [Here](https://github.com/flor14/tutorials) you have some examples of tutorials created with this framework. 

After one busy year that included the end of my PhD finally I have some time to make a contribution to the community about how to build these tutorials.

### Why to use Ines Montani framework?

1- [Ted Laderas](https://twitter.com/tladeras) has written some *"pros and cons"* of using this framework in this [post](https://education.rstudio.com/blog/2020/03/r-bootcamp/) in the RStudio education blog explaining the differences between Ines' framework with *learnr* package. 

2 - Ines Montani documentation is really detailed. If you find problems in building the tutorial I strongly suggest you came back to [her repo](https://github.com/ines/course-starter-r). 

> Do you teach a class using R and have a course that wants to convert to a tutorial? A course designed to be taught in a classroom is not exactly the same as an online tutorial. In the book [Teaching Tech Together by Greg Wilson](https://teachtogether.tech/#s:online) you can read more about the differences. 

### Recipe for an interactive tutorial ðŸ“

#### 1. **Ingredients**

First, you have to divide your course into **chapters**. As a general rule there are 4 or 5 chapters in a tutorial. 

###### The chapters can have:

* Slides with explanatory text associated 

* Codeblock exercises 

* Multiple choise exercises


ðŸ¤– 

> You can use [decampr package](https://laderast.github.io/decampr/articles/from_scratch.html) to generate some of the basic file structures. 

#### 2. **Copy the repository** ðŸ

You should have an account on GitHub (it is free). If you do not know how to do this, please check the following [webpage](https://help.github.com/en/github/getting-started-with-github/signing-up-for-a-new-github-account). If you want more information about git and GitHub in relation to R, I recommend the online book [Happy git with R](htpps://www.happygitwithr.com) by [Jenny Bryan](https://twitter.com/JennyBryan).

[The course starter R repository](https://github.com/ines/course-starter-r) is on GitHub. You can get a copy using it as a [template](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-from-a-template).

> Remember that this framework is available for [Python](https://github.com/ines/course-starter-python) too.

#### 3. **Custom elements** ðŸ“¦

###### **Slides with text**

* ðŸ“ [**slides** folder](https://github.com/juliasilge/supervised-ML-case-studies-course/tree/master/slides)
  - The slides are markdown (.md) files. It is good idea to name the file according to the chapter number and order of appearance, for example **chapter2_01.md**.
  - How is the structure of the slides file? Ines described it [here](https://github.com/ines/course-starter-r)
  
###### **Codeblock**

* ðŸ“ [**exercises** folder](https://github.com/juliasilge/supervised-ML-case-studies-course/tree/master/exercises) 
  - Each exercise file has an associated a solution file (and ideally a test file)
  - Tests are not fully developed yet.
  - The names for each file should have the same reference number:
  
<center>
  
  ![The solutions and exercises are separated files, linked by the final number in the name of the file](https://res.cloudinary.com/flor/image/upload/c_scale,w_475/v1585163873/tutorial2_hbfvio.png)
</center>  

###### **Multiple choise exercises**

* ðŸ“ [**chapters** folder](https://github.com/juliasilge/supervised-ML-case-studies-course/tree/master/chapters)
  - There are not specific files for them, are generated inside each chapter file. 
  - Read more about them [in the documentation](https://github.com/ines/course-starter-r)

âš ï¸

> Remember to include an id if more than one choice question is present in one exercise! You have an example [here, in the second exercise](https://github.com/noamross/gams-in-r-course/edit/master/chapters/chapter2.md)  

###### **Chapters** 

* ðŸ“ [**chapters** folder](https://github.com/juliasilge/supervised-ML-case-studies-course/tree/master/chapters)
  - Each chapter is a markdown (.md) file. 
  - Chapter structure: you should include the name of the slides, exercises and solution files. 
  
  ![Example of files in the chapter folder](https://res.cloudinary.com/flor/image/upload/v1585062072/tutorial1_emry8n.png)

#### Do not forget ðŸ˜®

- Customize the [*meta.json* file](https://github.com/noamross/gams-in-r-course/blob/master/meta.json) with the information corresponding to your course.

- Add a profile picture and logo too! -> ðŸ“ [**static** folder.](https://github.com/noamross/gams-in-r-course/tree/master/static)

âš ï¸

>  Remember include the logo in .svg format! You can convert a .png or .jpg image to this format online


### 3. **Cooking!**ðŸ³

Have you added all your files to you repository? Now it is time to see if it works!

Remember to read the [Section: Setting up Binder](https://github.com/ines/course-starter-r) and checking that the file [*install.R*](https://github.com/juliasilge/supervised-ML-case-studies-course/blob/master/binder/install.R) has all the packages used in the tutorial -> ðŸ“ [**binder** folder.](https://github.com/juliasilge/supervised-ML-case-studies-course/tree/master/binder)

You will have to use [Binder](https://mybinder.org/) in your repo. This can take a while! â°

Meanwhile, you can start your account in [Netlify](https://www.netlify.com/) for the deploy as [Ines did](https://github.com/ines/course-starter-r), but this step could be skipped. Why to use netlify? [I found this blogpost of Yihui Xie](https://yihui.org/en/2017/06/netlify-instead-of-github-pages/) with an explanation. It is up to you!

As soon as you are using Netlify you will be able to visualize the changes that you are making in the tutorial. The code will not work in codeblock exercises until you use Binder in your repository.

#### 4. **Customization** ðŸ’

- [To add a summary and a course description as introduction](https://ines.github.io/course-starter-python/#introduction-on-homepage)
- [Change logo size ](https://github.com/noamross/gams-in-r-course/blob/master/src/styles/index.module.sass) modifying *width* argument after *.logo*
- [Change the colors](https://github.com/juliasilge/supervised-ML-case-studies-course/blob/master/theme.sass) Modify *theme.sass*
- [Add a licence badge!](https://creativecommons.org/licenses/) You have to add it in the [meta.json](https://github.com/noamross/gams-in-r-course/blob/master/meta.json) file. 

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.

#### 5. **Something is missing** 

âš ï¸ 

Remember that tests are not fully developed yet!. For more info, read [the last section of the documentation.](https://github.com/ines/course-starter-r)

### Bon appÃ©tit ðŸ½!

Now you have your online tutorial ready to feed the community! 

You can make a pull request to [this repository](https://github.com/flor14/tutorials) that collects all the courses generated with this framework and other useful material to build your own course.

## Thanks

I want to thank [Noam Ross](https://twitter.com/noamross), [Julia Silge](https://twitter.com/juliasilge), [Ines Montani](https://twitter.com/_inesmontani) and [Ted Laderas](https://twitter.com/tladeras) for deciding to leave the material of their courses for free.


