# Text summarization of a Travel blog and tweeting it to increase the reach and expand business.

In this Code Pattern We will demonstrate a methodology to summarize a blog using Watson Studio. We will make use of the existing Code Pattern [Text summarization and visualization using watson studio](https://github.com/IBM/text-summarization-and-visualization-using-watson-studio). You will get the details of the text summarization from the suggested code pattern. This Code Pattern focuses on extractive summarization of the travel blog, extracting keywords converting them into relevant hashtags and tweeting it on twitter. 

For the sake of an example to show how one can market and grow their business, we have taken an upcoming famous website [hostelgeeks.com](https://hostelgeeks.com/short-travel-stories/) where they share stories of the people who have travelled or visited the places listed in their travel blogs. Humans are fond of stories. Since childhood they have lots of memories to share which makes them happy. Sharing their experience with other people does two things. First any travel blog gives awareness to the travellers and also incites the desire to visit and have that experience too. Second it reviews and comments about any place from a credible source also decides the credibilty of that place which all the travellers look for before investing in any travel plans. So we ran text Summarization on the stories, converted them into meaningful impactful tweet and tweeted it using twitter API with relevant Hashtags.

[A Brief about Text Summarization](https://machinelearningmastery.com/gentle-introduction-text-summarization)

When the reader has completed this code pattern, they will understand how to:

* Quickly summarize the text from documents & news feeds.
* Create topic modeling on the text to extract important topics.
* Create visualizations for better understanding of the data.
* Interpret the summary and visualization of the data.
* Tweet it on twitter.

# Architecture Diagram

![](https://github.com/Neha-Setia/summarizingTheArticleAndTweetingIt/blob/master/doc/source/images/architecture.png)

## Flow

1.  User logs into Watson Studio, creates an instance which includes object storage.
2.  User uploads the data file to the object storage.
3.  User imports a Jupyter Notebook from the URL.
4.  User runs the processing techniques & creates a statistical model for topics in the notebook.
5.  User explores the visualization in the notebook and can export the output to object storage.


# Watch the Video

[![](http://img.youtube.com/vi/oxDIXrDcQxc/hqdefault.jpg)](https://youtu.be/oxDIXrDcQxc)


# Steps

Follow these steps to setup and run this code pattern. The steps are
described in detail below.

1. [Create an account with IBM Cloud](#1-create-an-account-with-ibm-cloud)
1. [Create a new Watson Studio project](#2-create-a-new-watson-studio-project)
1. [Create the notebook](#3-create-the-notebook)
1. [Add the data](#4-add-the-data)
1. [Get access tokens and consumer key to use Twitter Api.](#5-get-access-tokens-and-consumer-key-to-use-twitter-api)
1. [Sample Output](#6-sample-output)
1. [Future Scope and Extension](#7-future-scope-and-extension)
1. [More Enterprise Use Cases](#8-more-enterprise-use-cases)


## 1. Create an account with IBM Cloud

Sign up for IBM [**Cloud**](https://console.bluemix.net/). By clicking on create a free account you will get 30 days trial account.

## 2. Create a new Watson Studio project

Sign up for IBM's [Watson Studio](http://dataplatform.ibm.com/). 

Click on `New project` and select `Data Science` as per below.

![](https://github.com/IBM/text-summarization-and-visualization-using-watson-studio/blob/master/doc/source/images/new_project.png)

Define the project by giving a Name and hit `Create`.

![](https://github.com/IBM/text-summarization-and-visualization-using-watson-studio/blob/master/doc/source/images/define_project.png)

By creating a project in Watson Studio a free tier ``Object Storage`` service will be created in your IBM Cloud account.

## 3. Create the notebook

* Open [IBM Watson Studio](https://dataplatform.ibm.com).
* Click on `Create notebook` to create a notebook.
* Select the `From URL` tab.
* Enter a name for the notebook.
* Optionally, enter a description for the notebook.
* Enter this Notebook URL:
  https://github.com/IBM/tweet-travel-blog-summary/blob/master/notebook/Text_Summarize_and_Tweet.ipynb
* Select the runtime (1vCPU and 4GBRAM)
* Click the `Create` button.

![](https://github.com/IBM/text-summarization-and-visualization-using-watson-studio/blob/master/doc/source/images/create_notebook.PNG)

## 4. Run the notebook

When a notebook is executed, what is actually happening is that each code cell in
the notebook is executed, in order, from top to bottom.

Each code cell is selectable and is preceded by a tag in the left margin. The tag
format is `In [x]:`. Depending on the state of the notebook, the `x` can be:

* A blank, this indicates that the cell has never been executed.
* A number, this number represents the relative order this code step was executed.
* A `*`, this indicates that the cell is currently executing.

There are several ways to execute the code cells in your notebook:

* One cell at a time.
  * Select the cell, and then press the `Play` button in the toolbar.
* Batch mode, in sequential order.
  * From the `Cell` menu bar, there are several options available. For example, you
    can `Run All` cells in your notebook, or you can `Run All Below`, that will
    start executing from the first cell under the currently selected cell, and then
    continue executing all cells that follow.


## 5. Get access tokens and consumer key to use Twitter Api.
* Go to `https://developer.twitter.com/` and sign in using twitter login ID. If you don't have login credentials, then sign up.
* Click on `Apps` (top right of the navigation bar)
![](doc/source/images/apps.png)

* Click on `Create an app` button.
![](doc/source/images/createanapp.png)

* Follow the process, answer the questions and it should create your app.
![](doc/source/images/appcreationprocess.png)

* Click on the `Details` button and then click on `Keys and Tokens` and get the access tokens and consumer keys.
![](doc/source/images/tweeted.png)

![](doc/source/images/keysandtokens.png)

## 6. Sample Output

Lets look at the summarization of the document. We can observe that all the key pointers are included in the summary. The text ranking algorithm has produced good results. 

```
I dislike entering book shops. Every time I walk into a book shop, I will end up
buying one. I entered an international bookshop in Example, Barcelona, while
looking for some cool things to do in Barcelona. And as expected, a book named
"The dead alleys of Barcelona" got my attention, a crime novel. Long story shot:
I bought it, went home, and started reading. In this book, the author Stefanie
Kremser talks about a special part of El Born, downtown Barcelona. She describes
this magical square, this narrow street the main character lived in. I didn't
know this exact street, and I was curious. I went downtown, wandered around the
square and saw this café with the few tables on the terrace. Until today, 7 years
later, it is still my favorite café in Barcelona – thanks to this book! – – –
This Short Travel Story was written by Matt, the guy behind Hostelgeeks. Here at
Hostelgeeks we award and collect 5 Star Hostels around the world. Fancy more coffee?
Find the 13 best coffee shops in Barcelona here. Barcelona is our home. You can
find our best-kept secret tips for Barcelona as well as 23 fun things to do. It
also includes our favorite Café in Barcelona. Our hottest tip for Barcelona?
Rent a Red Vespa (www.via-vespa.com) to get around easily.  Your email address
will not be published.
```

As we can see in the below image, the important words in the corpus have been highlighted which will help in inference of the data. Wordclouds are beautifully insightful with pros and cons. Word clouds can allow you to share back results from research in a way that does not require an understanding of the technicalities. Some of the pros are below.
* It reveals the essential. 
* They delight and provide emotional connection. 
* They are fast & engaging. 
As observed, skilled interpretation is what provides the beautiful insights. 

![](https://github.com/IBM/text-summarization-and-visualization-using-watson-studio/blob/master/doc/source/images/results_1.png)

Latent Dirichlet Allocation (LDA) is a probabilistic model with interpretable topics. Topic modeling is one of the most popular NLP techniques with several real-world applications such as dimensionality reduction, text summarization, recommendation engine, etc. To visualize our topics in a 2-dimensional space we will use the pyLDAvis library. This visualization is interactive in nature and displays topics along with the most relevant words.

on the running the cell with command 
```python
status = api.update_status(tweet_with_summary_hashtags)
print(status.id) 
```

you will get a code which indicates the tweet with hashtags has been tweeted.

![](doc/source/images/tweeted.png)


# 7. Future Scope and Extension

There are two main approaches to summarization:

~~Extractive summarization~~: it works by selecting the most meaningful sentences in an article and arranging them in a comprehensive manner. This means the summary sentences are extracted from the article without any modifications.

**Abstractive summarization: it works by paraphrasing its own version of the most important sentence in the article.**

There are also two scales of document summarization:

~~Single-document summarization~~ : the task of summarizing a standalone document. Note that a ” document” could refer to different things depending on the use case (URL, internal PDF file, legal contract, financial report, email, etc.).

**Multi-document summarization** the task of assembling a collection of documents (usually through a query against a database or search engine) and generating a summary that incorporates perspectives from across documents.

The Extractive Single Document Summarization and tweeting of the same has been showcased in this Code Pattern. The developers can further extend this Code Pattern to Abstractive Single Document,  Abstractive Multi-Document and Extractive Multi-Document Summarization. One of the challenges with these summarizations is that it is hard to generalize. For example, summarizing a news article is very different to summarizing a financial earnings report. 

There are two common metrics any summarizer attempts to optimize:
* Topic coverage: does the summary incorporate the main topics from the document?
* Readability: do the summary sentences flow in a logical way?

Thus the developers can further extend this Code Pattern to optimize it for other specific enterprise applications. The developers can read the following papers and blogs to do so.

- [Improving Abstraction in Text Summarization](https://aclweb.org/anthology/D18-1207)
- [An Optimization Text Summarization Method Based on Naïve Bayes and Topic Word for Single Syllable Language ](http://www.m-hikari.com/ams/ams-2014/ams-1-4-2014/haAMS1-4-2014.pdf)
-[Evolutionary Algorithm for Extractive Text Summarization](https://www.researchgate.net/publication/220518077_Evolutionary_Algorithm_for_Extractive_Text_Summarization)
-[Biogeography-Based Optimization Algorithm for Automatic Extractive Text Summarization](https://www.researchgate.net/publication/321918057_Biogeography-Based_Optimization_Algorithm_for_Automatic_Extractive_Text_Summarization)
-[A survey of multiple types of text summarization with their satellite contents based on swarm intelligence optimization algorithms](https://www.sciencedirect.com/science/article/pii/S0950705118304593)
- **[CORNELL NEWSROOM ](https://summari.es/)**

# 8.More Enterprise Use Cases

Companies producing long-form content, like whitepapers, e-books and blogs, might be able to leverage summarization to break down this content and make it sharable on social media sites like Twitter or Facebook. This would allow companies to further re-use existing content and also spread awareness amongst their employees.

Other Examples:
* Goodreads - analyse all the reviews of the book written by users, create summary and tweet it. The new users dont have to go through all the review comments.
* Amazon Product Reviews- analyse all the reviews of the products written by users, create summary and tweet it. This will help the new users to make an informed decision without going through all the review comments. 
Similarly, it can be used as :
* Internal Company Knowledge Summarizer. 
* Event summarizer.  
* Meeting summarizer. 
* Slack Group Chat Summarizer.
* Patent research.

# Troubleshooting

[See DEBUGGING.md.](DEBUGGING.md)

# License

This code pattern is licensed under the Apache Software License, Version 2.  Separate third party code objects invoked within this code pattern are licensed by their respective providers pursuant to their own separate licenses. Contributions are subject to the Developer [Certificate of Origin, Version 1.1 (DCO)](https://developercertificate.org/) and the [Apache Software License, Version 2](http://www.apache.org/licenses/LICENSE-2.0.txt).

ASL FAQ link: http://www.apache.org/foundation/license-faq.html#WhatDoesItMEAN
