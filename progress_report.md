Progress report
====
Project prep
---
2/7/19

Created Github repository for project. Added a Readme file, a placeholder License file, and my Project plan and Progress Report.

Progress report #1
---
2/21/19

I began investigating the dataset using Pandas. In my Jupyter notebook file [` progress_report1.ipnyb` ](https://github.com/Data-Science-for-Linguists-2019/Blog-Sentiment-Analysis/blob/master/progress_report1.ipynb), I created a DataFrame for the blogs and compiled some basic statistics: the number of blogs per author, gender, industry, and astrological sign. I also created data visualizations for each stat. After looking at basic stats, I did some preliminary exploration into the blog texts by looking at token frequencies and average blog length.

__Data sharing plan:__

The Blog Authorship Corpus's license states that it may be freely used for noncommercial purposes. From this, it seems that it would be okay for me to reupload the data onto Github. However, since there are 681,284 blog posts, that is maybe too much data for me to share with my classmates for this project. I created a smaller subset of the data, with 100 randomly selected blog posts.

The subset is titled [`mini_data.csv`](https://github.com/Data-Science-for-Linguists-2019/Blog-Sentiment-Analysis/blob/master/data_samples/mini_data.csv), and can be found in the [`data_samples`](https://github.com/Data-Science-for-Linguists-2019/Blog-Sentiment-Analysis/tree/master/data_samples) folder of my project repo.

Progress report #2
---
3/19/19

I corrected some of my mistakes in my previous data exploration. In my Jupyter notebook file [`progress_report_part2.ipnyb`](https://github.com/Data-Science-for-Linguists-2019/Blog-Sentiment-Analysis/blob/master/progress_report_part2.ipynb), I continued looking at basic stats and created some more graphs. I began investigating word frequency by industry and topic clustering.

__Data sharing plan:__

I have decided since the Blog Authorship Corpus is freely available on the web, I will not repost it in its entirety. I will keep it to just the subset I posted.

__License:__

I picked GNU General Public License for my code, which allows people to modify and distribute my code as long as they disclose the source and continue to use the same license.

Progress report #3
---
4/9/19

In my first Jupyter notebook file [`progress_report_part3.ipnyb`](https://github.com/Data-Science-for-Linguists-2019/Blog-Sentiment-Analysis/blob/master/progress_report_part3.ipynb), I used VADER (Valence Aware Dictionary and sEntiment Reasoner) to explore sentiment in the Blog Authorship Corpus. I also created some data visualizations for sentiment using a smaller subset of the data. I then saved my dataframe and transferred my work over to R, where I tried out some data visualizations for the whole dataset and some stats things. I created a second Jupyter notebook file [`progress_report_part3b.ipnyb`](https://github.com/Data-Science-for-Linguists-2019/Blog-Sentiment-Analysis/blob/master/progress_report_part3b.ipynb) with an R kernel. I did not find any significant relationships between any of the demographic info and polarity, but it was still a worthwhile exploration.

I am not planning on changing my data sharing plan. I will not push the CSV file with the polarity scores, since I think it is unnecessary. 
