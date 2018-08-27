# bigdatadayla
Big Data Day LA demo

# When Rotten Tomatoes Isn't Enough: Twitter Sentiment Analysis with DSE

## Setup Instructions

* Create a Twitter Account and get API access: https://developer.twitter.com/en/docs/ads/general/guides/getting-started.html

### Running inside a VM

* Install DSE https://docs.datastax.com/en/install/doc/install60/installTOC.html
* Start DSE Analytics Cluster: dse cassandra -k #Must use -k option for Analytics
* Set and Source Twitter enviroment variables in shell you will start Jupyter from
  * CONSUMER_KEY 
  * CONSUMER_SECRET 
  * ACCESS_TOKEN 
  * ACCESS_TOKEN_SECRET
* Using Python 2.7
* Using DSE Analytics 6
* Using latest verion of Jupyter
* Install Anaconda and Jupyter #Anaconda is not required but will make installing jupyter easier 
* Find full path to <>/dse-6.0.1/resources/spark/python/lib/pyspark.zip
* Find full path to <>/dse-6.0.1/resources/spark/python/lib/py4j-0.10.4-src.zip
* Start Jupyter with DSE to get all environemnt variables: dse exec jupyter notebook
* !pip install cassandra-driver
* !pip install tweepy 
* !pip install pattern 
* !pip install panadas
* Counter-intuitive don't install pyspark!!

### Running with Docker
* Make sure you have Docker installed and are logged in
* Create a file to hold environment variables
  * CONSUMER_KEY=...
  * CONSUMER_SECRET=...
  * ACCESS_TOKEN=...
  * ACCESS_TOKEN_SECRET=...
* Run DSE and Jupyter using docker-compose
  * (from repo directory, where docker-compose.yaml is located) **docker-compose up -d**
* Jupyter notebook server will be accessible at http://localhost:8888
  * Check log of Jupyter container to get login token
    *docker logs bigdatadayla_jupyter_1 

