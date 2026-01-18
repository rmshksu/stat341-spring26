---
layout: page
title: Homework 1
permalink: /assignments/homework-1
parent: Assignments
nav_order: 1
---
  
# Homework 1
  
The goal of this assignment is to introduce you to R, RStudio, and R markdown. We will be using these three programs throughout the course. You will be using these programs to make assignments (and other documents) that involve reporting the results obtained from R easily reproducible. In the most basic sense, this is equivalent to “showing your work” as you would for assignments with analytical components.

- As I mentioned in class, using R, RStudio, and R markdown is not required for this class. You are free to use whatever programming language you are familiar with as long as it is capable of doing basic statistical functions and making documents that enable your work to be reproducible. If you do not plan on using R, RStudio, and R markdown, please send me an email that explains what software you are using and why you want to use it. I do reserve the right to deny the use of certain software if I think it is incapable of doing what is required for this class. If you choose not to use R, RStudio, and R markdown, you must complete the assignment using the software of your choice.

1. Install R and RStudio.

2. In RStudio, create a new R Markdown file. Change the default output format to PDF.

3. Within the new R markdown file, delete the existing code and text (be carful to retain the top four lines which R markdown requires). Using the code below, download the annual $\text{CO}_2$ concentrations from Mt. Loa. With the code provided, plot the data.
  
```
url <- "https://gml.noaa.gov/webdata/ccgg/trends/co2/co2_annmean_mlo.txt" 
df <- read.table(url,header=FALSE) 
colnames(df) <- c("year","meanCO2","unc")

plot(x = df$year, y = df$meanCO2, xlab = "Year", ylab = expression("Mean annual "*CO[2]*" concentration"),  main="your name here",col="blue")
```

4. Change the plot title from “your name here” to your actual name. Change the color of the points from blue to a color of your choice. Knit the file to HTML or pdf and save the file as Yourlastname_Assignment1 (e.g., Sholl_Assignment1). Upload this file to Canvas by 11:59 pm on Friday 01/23/26.

