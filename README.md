# Data-Science-Capstone-Final-Project

(https://github.com/akselix/capstone_swiftkey)
  
This project was the final part of a 10 course Data Science track by Johns Hopkins University on Coursera. It was done as an industry partnership with SwiftKey. The job was to clean and analyze a large corpus of unstructured text and build a word prediction model and use it in a web application.
  
More info here: (http://rpubs.com/akselix/word_prediction)

### Overview

The goal of this exercise is to create a product to highlight the prediction algorithm that I have built and to provide an interface that can be accessed by others. For this project must submit:

1. A Shiny app that takes as input a phrase (multiple words) in a text box input and outputs a prediction of the next word.
2. A slide deck consisting of no more than 5 slides created with R Studio Presenter (https://support.rstudio.com/hc/en-us/articles/200486468-Authoring-R-Presentations) pitching your algorithm and app as if you were presenting to your boss or an investor.
This repository contains the ui.R and server.R files for the developed Shiny Application as well as the RStudio Presenter files for the Data Science Capstone Course Project.


## About Data

The corpora are collected from publicly available sources by a web crawler. The crawler checks for language, so as to mainly get texts consisting of the desired language*.

Each entry is tagged with it's date of publication. Where user comments are included they will be tagged with the date of the main entry.

Each entry is tagged with the type of entry, based on the type of website it is collected from (e.g. newspaper or personal blog) If possible, each entry is tagged with one or more subjects based on the title or keywords of the entry (e.g. if the entry comes from the sports section of a newspaper it will be tagged with "sports" subject).In many cases it's not feasible to tag the entries (for example, it's not really practical to tag each individual Twitter entry, though I've got some ideas which might be implemented in the future) or no subject is found by the automated process, in which case the entry is tagged with a '0'.

To save space, the subject and type is given as a numerical code.

Once the raw corpus has been collected, it is parsed further, to remove duplicate entries and split into individual lines. Approximately 50% of each entry is then deleted. Since you cannot fully recreate any entries, the entries are anonymised and this is a non-profit venture I believe that it would fall under [Fair Use](https://web-beta.archive.org/web/20160930083655/http://en.wikipedia.org/wiki/Fair_use).

* You may still find lines of entirely different languages in the corpus. There are 2 main reasons for that:1. Similar languages. Some languages are very similar, and the automatic language checker could therefore erroneously accept the foreign language text.2. "Embedded" foreign languages. While a text may be mainly in the desired language there may be parts of it in another language. Since the text is then split up into individual lines, it is possible to see entire lines written in a foreign language.Whereas number 1 is just an out-and-out error, I think number 2 is actually desirable, as it will give a picture of when foreign language is used within the main language.

Content archived from heliohost.org on September 30, 2016 and retrieved via Wayback Machine on April 24, 2017. https://web-beta.archive.org/web/20160930083655/http://www.corpora.heliohost.org/aboutcorpus.html 

Note : At this Task I use only English Text

## Review criteria

#### Data Product

- Does the link lead to a Shiny app with a text input box that is running on shinyapps.io?
- Does the app load to the point where it can accept input?
- When you type a phrase in the input box do you get a prediction of a single word after pressing submit and/or a suitable delay for the model to compute the answer?
- Put five phrases drawn from Twitter or news articles in English leaving out the last word. Did it give a prediction for every one?

#### Slide Deck

- Does the link lead to a 5 slide deck on R Pubs?
- Does the slide deck contain a description of the algorithm used to make the prediction?
- Does the slide deck describe the app, give instructions, and describe how it functions?
- How would you describe the experience of using this app?
- Does the app present a novel approach and/or is particularly well done?
- Would you hire this person for your own data science startup company?

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
  
