# elasticsearch-hints

These links are outcome of 4+ years of tuning/running our ES clusters (on premise and in a cloud).

> This list is not in the active development. Partially merged into https://github.com/dzharii/awesome-elasticsearch


## Internals

- [A Dive into the Elasticsearch Storage](https://www.found.no/foundation/dive-into-elasticsearch-storage/)
  
   In this article we'll investigate the files written to the data directory by various parts of Elasticsearch. We will look at node, index and shard level files and give a short explanation of their contents in order to establish an understanding of the data written to disk by Elasticsearch.


## Java tuning

- [Elasticsearch Java Virtual Machine settings explained](http://jprante.github.io/2012/11/28/Elasticsearch-Java-Virtual-Machine-settings-explained.html)
- [Tuning Garbage Collection for Mission-Critical Java Applications](http://blog.mgm-tp.com/2013/03/garbage-collection-tuning/)
- [G1: One Garbage Collector To Rule Them All](http://www.infoq.com/articles/G1-One-Garbage-Collector-To-Rule-Them-All)
- [Use Lucene’s MMapDirectory on 64bit platforms, please!](http://blog.thetaphi.de/)
- [Black Magic cookbook](http://product.hubspot.com/blog/g1gc-tuning-your-hbase-cluster)
- [G1GC Fundamentals: Lessons from Taming Garbage Collection](http://product.hubspot.com/blog/g1gc-fundamentals-lessons-from-taming-garbage-collection)
- [JVM Garbage Collector settings
investigation](https://tigase.tech/attachments/download/4808/GC-result.pdf)

    Comparison of jvm gc. Fantastic job!
    
- [Garbage Collection Settings for Elasticsearch Master Nodes](https://dzone.com/articles/garbage-collection-settings-for-elasticsearch-mast)
    
    Fine tunine your garbage collector
    
- [Understanding G1 GC Log Format](https://dzone.com/articles/understanding-g1-gc-log-format)

    To tune and troubleshoot G1 GC enabled JVMs, one must have a proper understanding of G1 GC log format. This article walks through key things that one should know about the G1 GC log format.

How to start using G1
```
#ES_JAVA_OPTS=""
ES_JAVA_OPTS="-XX:-UseParNewGC -XX:-UseConcMarkSweepGC -XX:+UseG1GC"

```


## Durability & reliability

- [Call me maybe: Elasticsearch](https://aphyr.com/posts/317-call-me-maybe-elasticsearch)

   In this post, we’ll explore Elasticsearch’s behavior under various types of network failure.

- [Call me maybe: Elasticsearch 1.5.0](https://aphyr.com/posts/323-call-me-maybe-elasticsearch-1-5-0)

   Data-loss scenarios

- [Transactions in Elasticsearch](https://blog.codecentric.de/en/2014/10/transactions-elasticsearch/)

   How to achieve transactions in Elasticsearch?


## Performance

- [Elasticsearch Refresh Interval vs Indexing Performance](http://blog.sematext.com/2013/07/08/elasticsearch-refresh-interval-vs-indexing-performance/)

   Because refreshing is expensive, one way to improve indexing throughput is by increasing refresh_interval. Less refreshing means less load, and more resources can go to the indexing threads. How does all this translate into performance? Below is what our benchmarks revealed when we looked at it 

- [A-Z Guide on Scaling Elasticsearch](https://qbox.io/blog/a-z-guide-on-scaling-elasticsearch)

   In this article we will discuss the system settings in detail. This will guide you on the parameters and values to be considered in various levels including the operating system (we are considering the Unix-based systems here). Focus will also be given to the memory settings in Elasticsearch, and we will look even deeper into the heap memory management and fine tuning of the same.

## Monitoring

- [Top 10 Elasticsearch Metrics to Watch](http://blog.sematext.com/2015/05/05/top-10-elasticsearch-metrics-to-watch/)

   This should be especially helpful to those readers new to Elasticsearch, and also to experienced users who want a quick start into performance monitoring of Elasticsearch.

- [How to monitor Elasticsearch performance](https://www.datadoghq.com/blog/monitor-elasticsearch-performance-metrics/)

   Very good article from Datadog
   
- [What should you monitor](https://support.lucidworks.com/hc/en-us/articles/201298247-What-should-you-monitor)
   
   Good checklist (with the explanations)

## Best practices

- [Elasticsearch Indexing Performance Cheatsheet](https://blog.codecentric.de/en/2014/05/elasticsearch-indexing-performance-cheatsheet/)
- [Six Ways to Crash Elasticsearch](https://www.found.no/foundation/crash-elasticsearch/)
- [Playing HTTP Tricks with Nginx](https://www.elastic.co/blog/playing-http-tricks-nginx)
- [Elasticsearch Tuning Plan](https://gist.github.com/mrflip/5366376)

   Nice check list

- [Choosing a fast unique identifier (UUID) for Lucene](http://blog.mikemccandless.com/2014/05/choosing-fast-unique-identifier-uuid.html)
  
   If have your own natural ID for each document, try to pick an ID that is friendly to Lucene. 

## Books

*In order of my personal preferences*

- [Relevant Search](https://www.manning.com/books/relevant-search) - best book available on the markert
- [Deep Learning for search](https://www.manning.com/books/deep-learning-for-search)
- [Mastering Elasticsearch - Second Edition](http://www.amazon.co.uk/Mastering-Elasticsearch-Second-Rafal-Kuc/dp/1783553790)
- [ElasticSearch Cookbook Second Edition](http://www.amazon.co.uk/ElasticSearch-Cookbook-Second-Edition-Alberto/)
- [Elasticsearch Server Second Edition](http://www.amazon.co.uk/Elasticsearch-Server-Second-Edition-Rogozi/dp/1783980524/) 

## Video

- ["Surviving Elasticsearch"](https://www.youtube.com/watch?v=gT-L6r37SPA)
- https://berlinbuzzwords.de/18/session/elasticsearch-index-management-paas-style-logging-system

## Reading

- https://medium.com/airbnb-engineering/listing-embeddings-for-similar-listing-recommendations-and-real-time-personalization-in-search-601172f7603e
- https://www.elastic.co/blog/modeling-data-for-fast-aggregations
- https://hackernoon.com/learning-to-rank-for-flight-itinerary-search-8594761eb867

