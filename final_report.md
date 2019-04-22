# Final report: Blog Sentiment Analysis
**[Eva Bacas](https://github.com/vnbcs) | [LING 1340](https://naraehan.github.io/Data-Science-for-Linguists-2019/) | April 26, 2019**

**Table of Contents:**
+ [1. Project overview](#1-project-overview)
  + 1.1 Introduction
  + 1.2 Goals of the project
  + 1.3 Process
+ [2. Data](#2-data)
  + [2.1 The Blog Authorship Corpus](#21-The-Blog-Authorship-Corpus)
  + 2.2 Reading and processing the data
  + 2.3 Overview of the corpus
+ [3. Analysis](#3-analysis)
  + 3.1 Word frequencies
  + 3.2 Topic modeling
  + 3.3 Sentiment analysis
+ [4. Conclusions](#4-conclusions)
  + 4.1 What I learned
  + 4.2 Setbacks and difficulties
  + 4.3 If I could do it again...
+ [5. Works Cited](#5-works-cited)


## 1. Project overview

### 1.1 Introduction
In this project, I investigated different ways to extract linguistic information from a corpus. I started my project without a clear idea in mind, but I found an interesting corpus of blogs and I wanted to explore analyses that I will hopefully use again in the future, as well as learn more about machine learning's linguistic applications.

### 1.2 Process

### 1.3 Setbacks and difficulties
Luckily, I did not have many issues reading in the data. However, I had a couple big difficulties while I was analyzing the data. First, my dataset is really large, and it did not occur to me to use a smaller subset of the data. This meant basically every text-based process took forever. I wish I had tweaked my [topic model](put something here) and gone back and tokenized with several different methods, but those processes just took so long. (Well, I actually did tokenize the whole dataset twice, but then I had another issue...)

When I was tokenizing the data for [the sentiment word frequency analysis](link to that), I read in the tokens to the data frame as a list. When I saved the data frame as a CSV, the list was put within another list, making the individual tokens inaccessible (at least, I couldn't figure out how access them). See [this thing](link something here) for more on that issue.

## 2. Data

### 2.1 The Blog Authorship Corpus

The Blog Authorship Corpus

### 2.2 Reading and processing the data

### 2.3 Overview of the Blog Authorship Corpus

There are 19,320 bloggers total and
#### Distribution of blogger ages
![png](images/graphs/distribution_of_blogger_ages.png)
*Description: This graph is a histogram of blogger ages. The ages range from 13 to 48, with no bloggers between the ages of 17 and 23 years old or 27 and 33 years old. The maximum value is at 17 years old. The graph is right skewed, meaning there are more younger bloggers than older bloggers.*

#### Top 10 industries by number of blogs
![png](images/graphs/top_10_industries_blog.png)
*Description: This graph is a histogram of the top 10 industries by number of blogs, excluding "Industry unknown". The maximum value is Student with over 150,000 blogs. The second greatest category is Technology, with around 40,000 blogs. The top 10 from greatest number of blogs to least is: Student, Technology, Arts, Education, Communications-Media, Internet, Non-Prpfot, Engineering, Law, and Publishing.*

#### Top 10 industries by blogger
![png](images/graphs/top_10_industries_blogger.png)
*Description: This graph is a histogram of the top 10 industries by number of bloggers, excluding "Industry unknown". The maximum value is Student with over 5000 blogs. This is over 25% of the total number of bloggers, 19320. There are slight differences between this graph and the graph of top 10 industries by number of blogs. Despite having more blogs total, there are less bloggers in the category Art than the subsequent category, Education.*

#### Distribution of blogger astrological signs
![png](images/graphs/distribution_of_blogger_signs.png)
*Description: This graph is a histogram of blogger astrological signs. The maximum value is the sign Virgo, though the distribution is fairly even. There are between 1400 and 1800 bloggers in every category.*

**Graph time**

## 3. Analysis

### 3.1 Word frequency

### 3.2 Topic modeling

### 3.3 Sentiment analysis

## 4. Conclusions

### 4.1 If I could do it again...

## 5. Works Cited
**Citations here**
