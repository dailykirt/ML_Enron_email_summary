# Enron Email Text Summarization
Capstone for Springboard 2019. ML techniques for summarizing emails using the Enron dataset. A flow chart summarizing the production workflow can be found [here.](https://github.com/dailykirt/ML_Enron_email_summary/blob/master/images/Text%20Summarizing%20Flow%20Chart.jpg) Currently a work in progress.

# Problem 
Email overload can be a difficult problem to manage for both work and personal email inboxes. With the average office worker receiving between 40 to 90 emails a day, it has become difficult to extract the most important information in an optimal amount of time. A system that can create concise and coherent summaries of all emails received within a timeframe can reclaim a large amount of time.

# Project Description
This project aims to apply extraction-based summarization methods to create a tool that can explore the Enron email dataset.

# Data
The Enron email dataset provides 150,000 emails from 150 users sent in a corporate environment. 
Source: https://www.cs.cmu.edu/~enron/
The dataset was processed by this notebook. 
The following preprocessing was done:
•	Parsing emails into constituent parts[Employee, Date, From, Subject, Body, Chain, Signature]
•	Removing non numerical characters, strings related to email attachments, and repeating whitespaces. 
•	Removed stopwords using the NLTK library. 

# Modeling
The extractive summarization algorithm is currently based on the TextRank Algorithm detailed in the article “An Introduction to Text Summarization using the TextRank Algorithm.”

# Web Interface
You can explore the Enron summaries [here](http://enron-emails.herokuapp.com/). Select an inbox, then press submit without date inputs to see the timeframe you can summarize. Then give the desired email timeframe to see summaries of all the emails in that period. You can also see the email where the summary was pulled from.
