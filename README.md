# Blog Sentiment Analysis

Created by [Eva Bacas](https://github.com/vnbcs).

## About

This is Eva's term project for [LING 1340: Data Science for Linguists](https://naraehan.github.io/Data-Science-for-Linguists-2019/). This project is an analysis of the sentiments and word frequencies in blogs, including variance across different author demographic groups.

## Data

This project uses the [Blog Authorship Corpus](http://u.cs.biu.ac.il/~koppel/BlogCorpus.htm).

J. Schler, M. Koppel, S. Argamon and J. Pennebaker (2006). Effects of Age and Gender on Blogging in Proceedings of 2006 AAAI Spring Symposium on Computational Approaches for Analyzing Weblogs. URL: http://www.cs.biu.ac.il/~schlerj/schler_springsymp06.pdf

## Directory

#### About the project:

+ [`README.md`](https://github.com/Data-Science-for-Linguists-2019/Blog-Sentiment-Analysis/blob/master/README.md)
  + 📍 You are here! This document contains a brief description of the project, link to the dataset, and a repository directory.
+ [`project_plan.md`](https://github.com/Data-Science-for-Linguists-2019/Blog-Sentiment-Analysis/blob/master/project_plan.md)
  + Description of the dataset and my initial project plan
+ [`progress_report.md`](https://github.com/Data-Science-for-Linguists-2019/Blog-Sentiment-Analysis/blob/master/progress_report.md)
  + Project updates for each [progress report](#jupyter-notebook-files)
+ [`Project_presentation.pdf`](https://github.com/Data-Science-for-Linguists-2019/Blog-Sentiment-Analysis/blob/master/Project_presentation.pdf) - [Click here to view on Google Slides](https://bit.ly/2IxJ8i1)
  + PDF version of my final project presentation
+ [`final_report.md`](https://github.com/Data-Science-for-Linguists-2019/Blog-Sentiment-Analysis/blob/master/final_report.md)
  + In-depth explanation of the project, with background information and interpretation of the analysis

#### Jupyter notebook files:

+ [`progress_report1.ipynb`](https://github.com/Data-Science-for-Linguists-2019/Blog-Sentiment-Analysis/blob/master/progress_report1.ipynb) - [Click here to view on nbviewer](https://nbviewer.jupyter.org/github/Data-Science-for-Linguists-2019/Blog-Sentiment-Analysis/blob/master/progress_report1.ipynb#)
  + In my first progress report, I read the CSV file into a data frame and explored the data. I calculated basic stats about blogger demographics, but I forgot to consider that there are multiple blogs per blogger.
+ [`progress_report_part2.ipynb`](https://github.com/Data-Science-for-Linguists-2019/Blog-Sentiment-Analysis/blob/master/progress_report_part2.ipynb) - [Click here to view on nbviewer](https://nbviewer.jupyter.org/github/Data-Science-for-Linguists-2019/Blog-Sentiment-Analysis/blob/master/progress_report_part2.ipynb)
  + In my second progress report, I continued exploring the data frame and corrected my issues from my first progress report. I began my analysis by looking at word frequencies and topic modeling.
+ [`progress_report_part3.ipynb`](https://github.com/Data-Science-for-Linguists-2019/Blog-Sentiment-Analysis/blob/master/progress_report_part3.ipynb) - [Click here to view on nbviewer](https://nbviewer.jupyter.org/github/Data-Science-for-Linguists-2019/Blog-Sentiment-Analysis/blob/master/progress_report_part3.ipynb)
  + In my third progress report, I explored sentiment analysis using [VADER](https://github.com/cjhutto/vaderSentiment) (Valence Aware Dictionary and sEntiment Reasoner). I categorized blogs as positive, negative, or neutral, and then investigated variation across blogger groups and most frequent words per sentiment category.
+ [`progress_report_part3b.ipynb`](https://github.com/Data-Science-for-Linguists-2019/Blog-Sentiment-Analysis/blob/master/progress_report_part3b.ipynb) - [Click here to view on nbviewer](https://nbviewer.jupyter.org/github/Data-Science-for-Linguists-2019/Blog-Sentiment-Analysis/blob/master/progress_report_part3b.ipynb)
  + This is a continuation of the third progress report. I switched to a new Jupyter notebook so I could use R. I attempted to create a mixed effects regression model using the demographic info as predictors and polarity score as an outcome.  It didn't work and nothing was significant.

#### Folders:

+ [`/data_samples`](https://github.com/Data-Science-for-Linguists-2019/Blog-Sentiment-Analysis/tree/master/data_samples)
  + Contains a 100 blog sample of the dataset
+ [`/images`](https://github.com/Data-Science-for-Linguists-2019/Blog-Sentiment-Analysis/tree/master/images)
  + PNG versions of all graphs and additional images in my project presentation and final report

#### Other files:

+ [`LICENSE.md`](https://github.com/Data-Science-for-Linguists-2019/Blog-Sentiment-Analysis/blob/master/LICENSE.md)
  + GNU General Public License v3.0
+ [`.gitignore`](https://github.com/Data-Science-for-Linguists-2019/Blog-Sentiment-Analysis/blob/master/.gitignore)
  + Prevents all my data from being uploaded

## Code

This code is licensed under the GNU General Public License v3.0.

## Guestbook

Please leave comments, suggestions, and questions in [my guestbook](https://github.com/Data-Science-for-Linguists-2019/Class-Plaza/blob/master/guestbooks/guestbook_eva.md).
