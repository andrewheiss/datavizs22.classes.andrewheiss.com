---
title: "Amounts and proportions"
linktitle: "4: Amounts and proportions"
date: "2022-06-20"
due_date: "2022-06-20"
due_time: "11:59 PM"
toc: true
menu:
  assignment:
    parent: Exercises
    weight: 4
type: docs
editor_options: 
  chunk_output_type: console
---

## Getting started

The New York City Department of Buildings (DOB) maintains a list of construction sites that have been categorized as "essential" during the city's shelter-in-place pandemic order. They've provided [an interactive map here](https://www1.nyc.gov/assets/buildings/html/essential-active-construction.html) where you can see the different projects. There's also a link there to download the complete dataset. 

For this exercise, you're going to use this data to visualize the amounts or proportions of different types of essential projects in the five boroughs of New York City (Brooklyn, Manhattan, the Bronx, Queens, and Staten Island). 

You'll be doing all your R work in R Markdown this time (and from now on). You should use an RStudio Project to keep your files well organized (either on your computer or on RStudio.cloud). Either create a new project for this exercise only, or make a project for all your work in this class.

You'll need to download one CSV file and put it somewhere on your computer or upload it to RStudio.cloud—preferably in a folder named `data` in your project folder. You can download the data from [the DOB's map](https://www1.nyc.gov/assets/buildings/html/essential-active-construction.html), or use this link to get it directly:

- [<i class="fas fa-file-csv"></i> `EssentialConstruction.csv`](/projects/04-exercise/data/EssentialConstruction.csv)

To help you, I've created a skeleton R Markdown file with a template for this exercise, along with some code to help you clean and summarize the data. Download that here and include it in your project:

- [<i class="fab fa-r-project"></i> `04-exercise.Rmd`](/projects/04-exercise/04-exercise.Rmd)

In the end, the structure of your project directory should look something like this:

```text
your-project-name\
  04-exercise.Rmd
  your-project-name.Rproj
  data\
    EssentialConstruction.csv
```

To check that you put everything in the right places, you can download and unzip this file, which contains everything in the correct structure:

- [<i class="fas fa-file-archive"></i> `04-exercise.zip`](/projects/04-exercise.zip)


## Task 1: Reflection

Write your reflection for the day's readings.


## Task 2: Essential pandemic construction

Make the following plots and briefly explain what they show:

- Show the count or proportion of approved projects by borough using a bar chart

- Show the count or proportion of approved projects by category using a lollipop chart

- Show the proportion of approved projects by borough and category simultaneously using a heatmap

[The example for today's session](/example/04-example/) will be *incredibly* helpful for this exercise. Reference it.

You don't need to make these super fancy, but if you're feeling brave, experiment with adding a `labs()` layer or changing fill colors with `scale_fill_manual()` or with viridis palettes. 

You'll need to insert your own code chunks where needed. Rather than typing them by hand (that's tedious and you might miscount the number of backticks!), use the "Insert" button at the top of the editing window, or type <kbd>ctrl</kbd> + <kbd>alt</kbd> + <kbd>i</kbd> on Windows, or <kbd>⌘</kbd> + <kbd>⌥</kbd> + <kbd>i</kbd> on macOS.

<img src="../../../../../../../img/assignments/insert-chunk-button.png" width="19%" />


## Turning everything in

When you're all done, click on the "Knit" button at the top of the editing window and create an HTML or Word version (or PDF if you've [installed **tinytex**](/resource/install/#install-tinytex)) of your document. Upload that file to iCollege.

<img src="../../../../../../../img/assignments/knit-button.png" width="30%" />
