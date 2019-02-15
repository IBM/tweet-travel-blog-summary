# Short title

Text summarization of a Travel blog and tweeting it with appropriate hashtags.

# Long title

Text summarization of a Travel blog and tweeting it to increase the reach and expand business.

# Author

* [Neha Setia](https://www.linkedin.com/in/nehasetia) ( <neha1221@in.ibm.com>)
* [Manjula Hosurmath](https://developer.ibm.com/code/advocates/manjula-hosurmath) (<mhosurma@in.ibm.com>)

# URLs

### Github repo

* https://github.com/IBM/tweet-travel-blog-summary

### Other URLs

* [![](http://img.youtube.com/vi/oxDIXrDcQxc/hqdefault.jpg)](https://youtu.be/oxDIXrDcQxc)


# Summary
Growing a real following on Twitter takes more than sending out Tweets whenever your company has a product being released or an upcoming event. It’s about engaging with your target audience and interacting with them. Hashtags are so darn important in doing so. This Code Pattern focuses on extractive summarization of the travel blog, extracting keywords converting them into relevant hashtags and tweeting it on twitter to expand their business through social media marketing.

# Technologies

* [Data Science](https://developer.ibm.com/code/technologies/data-science/): Systems and scientific methods to analyze structured and unstructured data in order to extract knowledge and insights.
* [Analytics](https://developer.ibm.com/code/technologies/analytics/): Analytics delivers the value of data for the enterprise.
* [Python](https://www.python.org/): Python is a programming language that lets you work more quickly and integrate your systems more effectively.
* [Text Ranking](https://pypi.org/project/gensim/): Gensim is a free Python library designed to automatically extract semantic topics from documents. The gensim implementation is based on the popular TextRank algorithm.
* [Word Cloud](https://pypi.org/project/wordcloud/): It is used for identifying and visualizing the key words in the document.
* [pyLDAvis](https://pypi.org/project/pyLDAvis/) : It is a Python library for interactive topic model visualization.

# Description

Successful Twitter marketing is powerful. You can unlock new opportunities to grow your business online. If Twitter is used well, it can drive tons of traffic to your website. But you need to be creative when crafting tweets to promote your blog posts, videos, and other content. 

For the sake of an example to show how one can market and grow their business, we have taken an upcoming famous website [hostelgeeks.com](https://hostelgeeks.com/short-travel-stories/) where they share stories of the people who have travelled or visited the places listed in their travel blogs. Humans are fond of stories. Since childhood they have lots of memories to share which makes them happy. Sharing their experience with other people does two things. First any travel blog gives awareness to the travellers and also incites the desire to visit and have that experience too. Second it reviews and comments about any place from a credible source also decides the credibilty of that place which all the travellers look for before investing in any travel plans. So we ran text Summarization on the stories, converted them into meaningful impactful tweet and tweeted it using twitter API with relevant Hashtags.

Associations can use hashtags to reach their target audience and to help members filter information. This Code Pattern focuses on extractive summarization of the travel blog, extracting keywords converting them into relevant hashtags and tweeting it on twitter to expand their business through social media marketing.


# Flow

# Architecture Diagram

![](https://github.com/Neha-Setia/summarizingTheArticleAndTweetingIt/blob/master/doc/source/images/architecture.png)

1.  User logs into Watson Studio, creates an instance which includes object storage.
2.  User uploads the data file to the object storage.
3.  User imports a Jupyter Notebook from the URL.
4.  User runs the processing techniques & creates a statistical model for topics in the notebook.
5.  User explores the visualization in the notebook and can export the output to object storage.

# Instructions

Follow these steps to setup and run this code pattern. The steps are
described in detail below.

1. [Create an account with IBM Cloud](#1-create-an-account-with-ibm-cloud)
1. [Create a new Watson Studio project](#2-create-a-new-watson-studio-project)
1. [Create the notebook](#3-create-the-notebook)
1. [Add the data](#4-add-the-data)
1. [Get access tokens and consumer key to use Twitter Api.](#5-get-access-tokens-and-consumer-key-to-use-twitter-api)
1. [Sample Output](#6-sample-output)


# Components and services

* [IBM Watson Studio](https://www.ibm.com/cloud/watson-studio): Analyze data using RStudio, Jupyter, and Python in a configured, collaborative environment that includes IBM value-adds, such as managed Spark.

* [IBM Cloud Object Storage](https://console.bluemix.net/catalog/services/cloud-object-storage): An IBM Cloud service that provides an unstructured cloud data store to build and deliver cost effective apps and services with high reliability and fast speed to market. This code pattern uses Cloud Object Storage.

* [Jupyter Notebooks](http://jupyter.org/): An open-source web application that allows you to create and share documents that contain live code, equations, visualizations and explanatory text.

# Related Links
* [Data Science](https://developer.ibm.com/code/technologies/data-science/)
* [Analytics](https://developer.ibm.com/code/technologies/analytics/)
* [Python](https://www.python.org/)
* [Jupyter Notebooks](http://jupyter.org/)
* [IBM Watson Studio](https://www.ibm.com/cloud/watson-studio)

# Announcement
Title -  Unlock new opportunities to grow your business through Twitter using Watson Studio.

Twitter’s Value for Marketing is not hidden from all of us. However, growing your Twitter account and turning it into an actual tool that generates leads and builds up your brand is a challenge. Growing a real following on Twitter takes more than sending out Tweets whenever your company has a product being released or an upcoming event. It’s about engaging with your target audience and interacting with them. Hashtags are so darn important in doing so. A hashtag is a label used on social media sites that make it easier to find information with a theme or specific content. Associations can use hashtags to reach their target audience and to help members filter information.

This code pattern has been designed to give a detailed description to developers who are keen on increasing their business through social media marketing. In this Code Pattern, we ran text Summarization on the stories, converted them into a meaningful impactful tweet and tweeted it using twitter API with relevant Hashtags.

[A Brief about Text Summarization](https://machinelearningmastery.com/gentle-introduction-text-summarization)

When the reader has completed this code pattern, they will understand how to:

* Quickly summarize the text from documents & news feeds.
* Create topic modeling on the text to extract important topics.
* Create visualizations for a better understanding of the data.
* Interpret the summary and visualization of the data.
* Tweet it on Twitter.

View the entire [Summarizing the article And tweeting it](https://github.com/IBM/tweet-travel-blog-summary/) Journey, including demos, code, and more!

