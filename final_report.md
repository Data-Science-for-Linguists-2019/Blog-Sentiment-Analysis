# Final report: Blog Sentiment Analysis
### **[Eva Bacas](https://github.com/vnbcs) | [LING 1340](https://naraehan.github.io/Data-Science-for-Linguists-2019/) | April 26, 2019**

### Table of Contents:
+ **[1. Project overview](#1-project-overview)**
  + [1.1 Introduction](#11-introduction)
  + [1.2 Process](#12-process)
  + [1.3 Setbacks and difficulties](#12-setbacks-and-difficulties)
+ **[2. Data](#2-data)**
  + [2.1 The Blog Authorship Corpus](#21-The-Blog-Authorship-Corpus)
  + [2.2 Reading and processing the data](#22-reading-and-processing-the-data)
  + [2.3 Overview of the corpus](#23-overview-of-the-corpus)
+ **[3. Analysis](#3-analysis)**
  + 3.1 Word frequencies
  + 3.2 Topic modeling
  + 3.3 Sentiment analysis
+ **[4. Conclusions](#4-conclusions)**
  + 4.1 What I learned
  + 4.2 If I could do it again...
+ **[5. Works Cited](#5-works-cited)**


## 1. Project overview

### 1.1 Introduction
In this project, I investigated different ways to extract linguistic information from a corpus. I started my project without clear goals in mind. I knew I wanted to explore analyses that I will hopefully use again in the future, as well as learn more about machine learning's linguistic applications. I narrowed my interests down into three big research questions:

+ What information can I get out of a text corpus?
+ How can I use machine learning to extract that information?
+ How can I show that information with data visualization?

I found an interesting corpus, [the Blog Authorship Corpus](http://u.cs.biu.ac.il/~koppel/BlogCorpus.htm), made of Google Blogger blogs from 2004, and started exploring the data. In addition to the textual data, each blog contained demographic information related to the blogger, which provided a chance for me to explore the corpus through a sociolinguistic lens. Along the way, I developed more specific research questions to focus on for this project:

+ What are the most frequent words? How does word frequency vary between groups of bloggers?
+ What topics are found in these blogs?
+ What sentiments are found in these blogs? How does sentiment vary between groups of bloggers?

### 1.2 Process

**Write stuff here**

### 1.3 Setbacks and difficulties

Luckily, I did not have many issues [reading in the data](#22-reading-and-processing-the-data). However, I had a couple big difficulties while I was analyzing the data. First, my dataset is really large, and it did not occur to me to use a smaller subset of the data. This meant basically every text-based process took forever. I wish I had tweaked my [topic model](put something here) a couple more times and gone back and tokenized with several different methods, but those processes just took so long. (Well, I actually did tokenize the whole dataset twice, but then I had another issue...)

When I was tokenizing the data for [the sentiment word frequency analysis](link to that), I added the tokens as a column to my data frame where each row is a list of tokens. When I saved the data frame as a CSV, the list was put within another list, making the individual tokens inaccessible (at least, I couldn't figure out how access them). See [this thing](link something here) for more on that issue. I put off further word frequency analysis since I thought it would be easy to come back to, but because of this issue, I was not able to do as much with word frequency as I wanted to.

## 2. Data

### 2.1 The Blog Authorship Corpus

[The Blog Authorship Corpus](http://u.cs.biu.ac.il/~koppel/BlogCorpus.htm) was published in 2006 by Schler, Koppel, Argamon and Pennebaker. The corpus is the collected posts of 19,320 bloggers gathered from blogger.com in August 2004.

![png](images/blogger_in_2004/blogger_create-blog_2004.png)
*Description: This image is a screenshot of Google Blogger in August 2004. This image can be viewed on the Internet Archive [here](https://web.archive.org/web/20040804083743/http://www.blogger.com/start).*

### 2.2 Reading and processing the data

I found a [CSV version of this dataset on Kaggle](https://www.kaggle.com/rtatman/blog-authorship-corpus), posted by [Dr. Rachael Tatman](http://www.rctatman.com/). The original version of this corpus was made up of XML files, with each file containing all the blogs for a given blogger. While processing XML files would be a useful skill to learn, I didn't want to spend a lot of time on data cleanup if I didn't have to.

I read the CSV in as a data frame and added columns for things like tokens, sentiment, and polarity score. I saved the modified data frame as a CSV as well. **put some links here**

### 2.3 Overview of the corpus

There are 19,320 bloggers total and 681,288 posts. For each blogger, the dataset provides their [gender](#gender), [age](#age), [industry](#industry), and [astrological sign](#astrological-sign).

#### Gender

The gender breakdown is 50% female and 50% male.

#### Age

To make a Google blogger account, bloggers be at least 13 years of age. The ages of the bloggers range from 13 to 48, with two strange gaps between 17 and 23 years old and 27 and 33 years old. [The mean age is ~23 years old](put a link here). Considering the authors controlled so well for blogger gender, this seems to be a weird oversight, especially for a dataset of this size.

#### Distribution of blogger ages
![png](images/graphs/distribution_of_blogger_ages.png)
*Description: This graph is a bar chart of blogger ages. The ages range from 13 to 48, with no bloggers between the ages of 17 and 23 years old or 27 and 33 years old. The maximum value is at 17 years old. The graph is right skewed, meaning there are more younger bloggers than older bloggers.*

#### Industry

Industry refers to the self-identified industry or career field of the blogger. This category was not required in order to create a Google Blogger account. Bloggers who did not list their industry are labeled "indUnk" (= industry unknown). Industry unknown makes up over 50% of the dataset (**fact check this when ur notebooks load**).

*If ur reading this before I finish none of my Jupyter notebooks are loading on my personal laptop, it's very fun*

#### Top 10 industries by number of blogs
![png](images/graphs/top_10_industries_blog.png)
*Description: This graph is a bar chart of the top 10 industries by number of blogs, excluding "industry unknown". The maximum value is Student with over 150,000 blogs. The second greatest category is Technology, with around 40,000 blogs. The top 10 from greatest number of blogs to least is: Student, Technology, Arts, Education, Communications-Media, Internet, Non-Prpfot, Engineering, Law, and Publishing.*

#### Top 10 industries by number of bloggers
![png](images/graphs/top_10_industries_blogger.png)
*Description: This graph is a bar chart of the top 10 industries by number of bloggers, excluding "Industry unknown". The maximum value is Student with over 5000 blogs. This is over 25% of the total number of bloggers, 19320. There are slight differences between this graph and the graph of top 10 industries by number of blogs. Despite having more blogs total, there are less bloggers in the category Art than the subsequent category, Education.*

#### Astrological sign

I did not expect astrological signs to be a significant factor in any of my analyses, since it is basically totally random. (Sorry, astrology fans.) Despite this, I did look at [sentiment variation across astrological signs](put a link here) just for fun.

#### Distribution of blogger astrological signs
![png](images/graphs/distribution_of_blogger_signs.png)
*Description: This graph is a bar chart of blogger astrological signs. The maximum value is at the sign Virgo, though the distribution is fairly even. There are between 1400 and 1800 bloggers in every category.*

## 3. Analysis

### 3.1 Word frequency

### 3.2 Topic modeling

### 3.3 Sentiment analysis

## 4. Conclusions

### 4.1 If I could do it again...

## 5. Works Cited
**Citations here**
