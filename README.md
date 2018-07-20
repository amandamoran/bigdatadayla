# bigdatadayla
Big Data Day LA demo

When Rotten Tomatoes Isn't Enough: Twitter Sentiment Analysis with DSE
Things To Setup

Create a Twitter Account and get API access: https://developer.twitter.com/en/docs/ads/general/guides/getting-started.html

Install DSE https://docs.datastax.com/en/install/doc/install60/installTOC.html

Start DSE Analytics Cluster: dse cassandra -k #Must use -k option for Analytics

Install Anaconda and Jupyter #Anaconda is not required but will make installing jupyter easier

Start Jupyter with DSE to get all environemnt variables: dse exec jupyter notebook

!pip install cassandra-driver

!pip install tweepy

!pip install pattern

Counter-intuitive don't install pyspark!!
 
