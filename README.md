# Enron Email Text Summarization
Capstone for Springboard 2019. ML techniques for summarizing emails using the Enron dataset.

# Problem 
Email overload can be a difficult problem to manage for both work and personal email inboxes. With the average office worker receiving between 40 to 90 emails a day, it has become difficult to extract the most important information in an optimal amount of time. A system that can create concise and coherent summaries of all emails received within a timeframe can reclaim a large amount of time.

# Project Description
This project aims to apply extraction-based summarization methods to create a tool that can explore the Enron email dataset.  A flow chart summarizing the production workflow can be found [here](https://github.com/dailykirt/ML_Enron_email_summary/blob/master/images/Text%20Summarizing%20Flow%20Chart.jpg).

# Data
Two separate datasets are used for this project. The Enron email dataset provides 150,000 emails from 150 users sent in a corporate environment and the BC3 Email Corpus that contains 40 email threads. The BC3 Email Corpus contains human summaries that can be used to test the accuracy of the machine learning generated summaries. The Enron email dataset lacks human summaries, but is used to demonstrate the practical application of automatic summarizations to a huge number of emails.

Enron emails source: https://www.cs.cmu.edu/~enron/
BC3 Email Corpus source: https://www.cs.ubc.ca/cs-research/lci/research-groups/natural-language-processing/bc3.html

Both datasets are processed in this [notebook](https://github.com/dailykirt/ML_Enron_email_summary/blob/master/notebooks/Process_Emails.ipynb).

# Modeling
The extractive summarization algorithm is currently based on the TextRank Algorithm detailed in the article “An Introduction to Text Summarization using the TextRank Algorithm.”. Model accuracy was measured using the [ROUGE metric](https://pypi.org/project/py-rouge/).

The ML model was created and tested in this  [notebook](https://github.com/dailykirt/ML_Enron_email_summary/blob/master/notebooks/Text_rank_summarization.ipynb).

# Web Interface
You can explore the Enron summaries [here](http://enron-emails.herokuapp.com/).
