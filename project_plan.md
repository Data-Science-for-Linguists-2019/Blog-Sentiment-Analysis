Project plan: Blog Sentiment Analysis
===
Summary
---
This project is an analysis of the sentiments and word frequencies in blogs, including variance across different author demographic groups.
Data
---
Dataset: The Blog Authorship Corpus

Authors:
J. Schler, M. Koppel, S. Argamon and J. Pennebaker (2006). Effects of Age and Gender on Blogging in Proceedings of 2006 AAAI Spring Symposium on Computational Approaches for Analyzing Weblogs.

URL: http://u.cs.biu.ac.il/~koppel/BlogCorpus.htm

Makeup:
Collected posts of 19,320 bloggers gathered from blogger.com in August of 2004.

Size: 681,288 posts, or 140 million+ words, with ~35 posts/7250 words per blogger

Blogger info: ID#, self-provided gender, industry, and astrological sign

Categories: all blogs fall into three age groups, with an equal number of male and female bloggers in each category
	"10s": 13-17, numbering 8240 bloggers
	"20s": 23-27, numbering 8086 bloggers
	"30s": 33-47, numbering 2994 bloggers

Language: English

Format: .csv
Analysis
---
I intend to map words/phrases to sentiments, for example, "great" to happy, "looking forward to" to excited, as well as overall positive and negative sentiment. I will use these mapping to judge the overall sentiment of individual blogs, authors, and variance across demographic groups. I will check judgments and revise my mappings as I go.

I would also like to look at word frequencies, and see how word frequencies vary across demographic groups. For example, new slang might only be used by bloggers in the 13-17 age range, or certain industry-specific words might only be used by people working in Agriculture.
