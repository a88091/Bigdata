# Topic Model
## The topic model analyze reviews of high rating NYC companies on Indeed. By LDA model, we tried to cluster all reviews based on hidden topics of each review.

Introduction

Indeed is the largest recruitment search engine serving not only America but also globally. This website is dedicated to improving the online job-hunting experience, striving to provide the most comprehensive and accurate recruitment information for job seekers, aggregating tens of millions of recruitment information from thousands of recruitment websites, newspapers, job agencies, company websites, etc. every day. 

The most powerful thing is that although there is no gorgeous page, the overall SEO structure of the website is quite perfect. Besides, the development of "API" for docking with various enterprises enables you to import job information into the list of the industry, whether you are an individual company or a job site that you want to expose. That is to say, for job seekers, you can usually use only one Indeed website to view and integrate information on dozens of websites. For talent seekers, powerful SEO and website flow can help you get more exposure and talent opportunities.

At the same time, Jobseeker can give comments and ratings on the company to show their working experience and other needs. Comments are usually written by text, and overall ratings are the integration of sub-ratings for five aspects: Job_balance, Compensation, Job_Security, Management, and Job_Culture. Through these evaluations, we can understand these companies more intuitively, and the company can better build and improve its internal systems according to these suggestions.

Topic Model

Topic Model is a technique to extract the hidden topics from large volumes of text. Latent Dirichlet Allocation(LDA) is a popular algorithm for topic modeling with excellent implementations in Python’s Gensim package. The challenge, however, is how to extract good quality of topics that are clear, segregated and meaningful. This depends heavily on the quality of text preprocessing and the strategy of finding the optimal number of topics.

We tried to deal with our text data as unsupervised data with topic modeling. In this step, our goal was to find hidden topics of employees’ reviews. At first, we thought there might be five or more topics to cluster employees describing sub ratings related topics since Indeed ask these employees to rank five different categories besides overall rating. Then, after discussion, we thought that because we only focus on the top 50 rated companies in New York City, the hidden topic might vary over a large range. Assume that there are two kinds of employees: one has positive opinions about their company and the other one doesn’t have. In this way, it’s obvious we would guess there will be only two topics hidden in employees’ reviews.
In summary, we tried to offer enterprises in New York City a reference that what do employees care the most based on each topic. By doing so, companies can compete better with peers in the human resources market and employees can benefit from their employers.

reference:https://www.machinelearningplus.com/nlp/topic-modeling-gensim-python/
