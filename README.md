# elasticsearch-hints

## Internals

- [A Dive into the Elasticsearch Storage](https://www.found.no/foundation/dive-into-elasticsearch-storage/)
  
   In this article we'll investigate the files written to the data directory by various parts of Elasticsearch. We will look at node, index and shard level files and give a short explanation of their contents in order to establish an understanding of the data written to disk by Elasticsearch.


## Java tuning

- [http://jprante.github.io/2012/11/28/Elasticsearch-Java-Virtual-Machine-settings-explained.html](Elasticsearch Java Virtual Machine settings explained)

- [http://blog.mgm-tp.com/2013/03/garbage-collection-tuning/](Tuning Garbage Collection for Mission-Critical Java Applications)

- [http://www.infoq.com/articles/G1-One-Garbage-Collector-To-Rule-Them-All](G1: One Garbage Collector To Rule Them All)
- [http://blog.thetaphi.de/](Use Lucene’s MMapDirectory on 64bit platforms, please!)


    In the following article we take a look at the state-of-the-art advanced GC algorithms and important tuning options and compare them for diverse real-world scenarios  

## Durability & reliability

- [https://aphyr.com/posts/317-call-me-maybe-elasticsearch](Call me maybe: Elasticsearch)

   In this post, we’ll explore Elasticsearch’s behavior under various types of network failure.

- [https://aphyr.com/posts/323-call-me-maybe-elasticsearch-1-5-0](Call me maybe: Elasticsearch 1.5.0)

   Data-loss scenarios

- [https://blog.codecentric.de/en/2014/10/transactions-elasticsearch/](Transactions in Elasticsearch)

   How to achieve transactions in Elasticsearch?


## Performance

- [http://blog.sematext.com/2013/07/08/elasticsearch-refresh-interval-vs-indexing-performance/](Elasticsearch Refresh Interval vs Indexing Performance)

   Because refreshing is expensive, one way to improve indexing throughput is by increasing refresh_interval. Less refreshing means less load, and more resources can go to the indexing threads. How does all this translate into performance? Below is what our benchmarks revealed when we looked at it 

## Monitoring

- [http://blog.sematext.com/2015/05/05/top-10-elasticsearch-metrics-to-watch/](Top 10 Elasticsearch Metrics to Watch)

   This should be especially helpful to those readers new to Elasticsearch, and also to experienced users who want a quick start into performance monitoring of Elasticsearch.

## Best practices

- [https://blog.codecentric.de/en/2014/05/elasticsearch-indexing-performance-cheatsheet/](Elasticsearch Indexing Performance Cheatsheet)
- [https://www.found.no/foundation/crash-elasticsearch/](Six Ways to Crash Elasticsearch)
- [https://www.elastic.co/blog/playing-http-tricks-nginx](Playing HTTP Tricks with Nginx)

## Books

*In order of my personal preferences*

- [http://www.amazon.co.uk/Mastering-Elasticsearch-Second-Rafal-Kuc/dp/1783553790](Mastering Elasticsearch - Second Edition)
- [http://www.amazon.co.uk/ElasticSearch-Cookbook-Second-Edition-Alberto/](ElasticSearch Cookbook Second Edition)
- [http://www.amazon.co.uk/Elasticsearch-Server-Second-Edition-Rogozi/dp/1783980524/](Elasticsearch Server Second Edition) 
