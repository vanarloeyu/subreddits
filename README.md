# Clustering Subreddits Using Unsupervised Machine Learning

## Executive Summary
Reddit is a website that proclaims itself as the "front page of the internet." Reddit is broken up into millions of subreddits wherein each covers a different topic. For example, /r/datascience/ is a subreddit for people to discuss data science. The notebook presents a study to determine the major themes or subreddits from reddit.com based on the title of threads. An aggregated list of thread titles and authors from a text file was used in the study. The file was preprocessed and cleaned by removing characters that are not word characters (e.g., punctuations and emojis) and foreign characters (e.g., 南部). TfidfVectorizer was used to make a vector representation of the titles. The TfidfVectorizer determines the importance of a set of words to a document by determining the frequency of occurence of words and penalizes the most frequenctly occuring words in the corpus. TruncatedSVD was used to get a reduced rank approximation of the titles for feature reduction to eliminate noise, synonymy, and polysemy. Kmeans clustering was used to determine the clusters formed based on the titles before and after using TruncatedSVD. Nine (9) clusters were formed from the vector from TF-IDF and six (6) clusters were formed after TruncatedSVD was used. Each cluster formed represent a community of similar titles or themes that may correspond to a possible subreddit. The titles assigned to each cluster are representative of the features or words that define the cluster. The clusters are able to capture the titles being discussed under the common theme in each cluster. Future directions of this algorithm can be extended as the engine of a forum moderator system. It can also be used for digital marketing targeting wherein similar words can be obtained based on the community being targeted.

<i> This research is implemented in fulfilment of the requirements of the Data Mining and Wrangling course of the Master of Science in Data Science under the Asian Institute of Management. </i>
