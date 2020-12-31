# Data-Science-Capstone-Final-Project

(https://github.com/akselix/capstone_swiftkey)
  
This project was the final part of a 10 course Data Science track by Johns Hopkins University on Coursera. It was done as an industry partnership with SwiftKey. The job was to clean and analyze a large corpus of unstructured text and build a word prediction model and use it in a web application.
  
More info here: (http://rpubs.com/akselix/word_prediction)

### Overview

The goal of this exercise is to create a product to highlight the prediction algorithm that I have built and to provide an interface that can be accessed by others. For this project must submit:

1. A Shiny app that takes as input a phrase (multiple words) in a text box input and outputs a prediction of the next word.
2. A slide deck consisting of no more than 5 slides created with R Studio Presenter (https://support.rstudio.com/hc/en-us/articles/200486468-Authoring-R-Presentations) pitching your algorithm and app as if you were presenting to your boss or an investor.
This repository contains the ui.R and server.R files for the developed Shiny Application as well as the RStudio Presenter files for the Data Science Capstone Course Project.


##### The developed Shiny app for the the assignment is available [here](https://samaaessa.shinyapps.io/CourseraDataScienceCapstoneCourseProject/)

##### The pitch presentation is available [here](https://rpubs.com/samaaessa/708816)


#### Runbook

The source coude files and presentation files are available on this GitHub repo

**Shiny app**
  
1. Data is preloaded into (corpus.RData)
  
2. getting-cleaning data.R
	- Contains functions used for load, preprocess, and save data
  
3. ./shiny/server.R
	- Contains the server side functions
  
4. ./shiny/ui.R
	- Handles the input/output
  
