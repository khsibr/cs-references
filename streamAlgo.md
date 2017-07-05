1. *General Background and Overview*
  * [Probabilistic Data Structures for Web Analytics and Data Mining](http://highlyscalable.wordpress.com/2012/05/01/probabilistic-structures-web-analytics-data-mining/) : A great overview of the space of probabilistic data structures and how they are used in approximation algorithm implementation.
  * [Models and Issues in Data Stream Systems](http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.106.9846)
  * [Philippe Flajolet’s contribution to streaming algorithms](https://speakerdeck.com/timonk/philippe-flajolets-contribution-to-streaming-algorithms) : A presentation by Jérémie Lumbroso that visits some of the hostorical perspectives and how it all began with Flajolet
  * [Approximate Frequency Counts over Data Streams](http://www.vldb.org/conf/2002/S10P03.pdf) by Gurmeet Singh Manku & Rajeev Motwani : One of the early papers on the subject.
  * [Methods for Finding Frequent Items in Data Streams](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.187.9800&rep=rep1&type=pdf) by Graham Cormode & Marios Hadjieleftheriou 
  * [The space complexity of approximating the frequency moments](http://www.tau.ac.il/~nogaa/PDFS/amsz4.pdf) by Noga Alon, Yossi Matias, Mario Szegedy : one of the most influential papers introducing succinctness in computing frequency moments  
  * [Cuckoo Filter: Practically Better Than Bloom](http://www.pdl.cmu.edu/PDL-FTP/FS/cuckoo-conext2014.pdf) by Bin Fan, David G. Andersen, Michael Kaminsky, Michael D. Mitzenmacher
  * [A Simple Algorithm for Finding Frequent Elements in Streams and Bags](http://www.cs.umd.edu/~samir/498/karp.pdf) by Karp, Shenker and Papadimitriou : used in Spark to find frequent items

2. [Hyperloglog and MinHash](http://tech.adroll.com/blog/data/2013/07/10/hll-minhash.html) : Implementation of a form of hyperloglog and adding capabilities of MinHash algorithm on to it which would enable to perform set intersections."While it does require extra processing power to deal with collecting all the minima, it’s possible to get satisfactory performance out of the structure for a relatively low storage or memory footprint" 

3. [Streaming/Sketching Conference from AK Tech](http://blog.aggregateknowledge.com/2013/05/23/foundation-capital-and-aggregate-knowledge-sponsor-streamingsketching-conference/) : Contains links to videos and slides from the speakers like Muthukrishnan who spoke about Count Min Sketch 

4. *Q-digest*
  * [Medians and Beyond: New Aggregation Techniques for Sensor Networks](http://www.cs.virginia.edu/~son/cs851/papers/ucsb.sensys04.pdf) : The paper that introduced q-digest for range queries and quantile approximation 
  * [Blog post on q-digest](http://papercruncher.com/2011/07/31/q-digest/)
  * [Blog post on approximate quantiles](http://www.prelert.com/blog/q-digest-an-algorithm-for-computing-approximate-quantiles-on-a-collection-of-integers/)
  * [The Art of Approximating Distributions](http://metamarkets.com/2013/histograms/#) : Histograms and Quantiles at Scale - an alternative approach to q-digest 
  
5. [t-digest](https://github.com/tdunning/t-digest) : A new data structure for accurate on-line accumulation of rank-based statistics such as quantiles and trimmed means. Ted Dunning's variant of Q-digest that does some improvements 

6. *Implementations*
  * [stream-lib](https://github.com/addthis/stream-lib) : A collection of Stream summarization and cardinality estimation algorithms like CM Sketch, Hyperloglog, Bloom Filters 
  * [Algebird from Twitter](https://github.com/twitter/algebird)
  * [streamDM - Data Mining for Spark Streaming](http://huawei-noah.github.io/streamDM/)

7. *Count-Min Sketch*
  * [An Improved Data Stream Summary: The Count-Min Sketch and its Applications](http://dimacs.rutgers.edu/~graham/pubs/papers/cm-full.pdf) - Cormode & Muthukrishnan : The paper that introduced count min sketch 
  * [Collection of information on Count Min Sketch](https://sites.google.com/site/countminsketch/)
  * [Count Min Sketch](http://dimacs.rutgers.edu/~graham/pubs/papers/cmencyc.pdf) by Cormode : Introductory paper 
  * [Streaming Algorithms and Sketches](http://blog.aggregateknowledge.com/2011/09/13/streaming-algorithms-and-sketches/) - Count Min Sketch on AK Tech Blog 
  * Muthukrishnan [talking](http://www.youtube.com/watch?v=OOZC4KCErN0) on Count Min Sketch at AK Tech conference 
  * [Sketch Techniques for Approximate Query Processing](http://people.cs.umass.edu/~mcgregor/711S12/sketches1.pdf) by Cormode 
  * [Sketching data structures](http://lkozma.net/blog/sketching-data-structures/) - a good overview of Bloom Filters and Count Min Sketch
  * [Sketching can improve linear regression](https://speakerdeck.com/timonk/sketching-as-a-tool-for-numerical-linear-algebra) and the [talk](http://www.youtube.com/watch?v=-7S9jNeY_R0) by David
  * [A Framework for Clustering Massive-Domain Data Streams](http://charuaggarwal.net/cskrevise.pdf) by Charu Aggarwal
  * [Streaming Anomaly Detection Using Randomized Matrix Sketching](http://www.cse.psu.edu/~kasivisw/randsketch.pdf) by Huang & Kasiviswanathan
  * [Time adaptive sketches for summarizing data streams](http://research.microsoft.com/en-us/um/people/mbilenko/papers/16-ada-sketches.pdf) by Anshumali Shrivastava et. al from Microsoft Research
  
8. *Surveys*
  * [References for Data Stream Algorithms](http://dimacs.rutgers.edu/~graham/pubs/papers/bristol.pdf) by Graham Cormode : an exhaustive set of references with explanations 
  * [Data Streams - Algorithms and Applications](http://www.amazon.com/Data-Streams-Applications-Foundations-Theoretical/dp/193301914X) by S. Muthukrishnan  :  This is an excellent monograph with surveys of all algorithms related to data streams. Also a free copy of the book is available from Muthu's web site at http://www.cs.rutgers.edu/~muthu/
  * [Synopses for Massive Data: Samples, Histograms, Wavelets, Sketches](http://www.nowpublishers.com/articles/foundations-and-trends-in-databases/DBS-004) by Graham Cormode1, Minos Garofalakis, Peter J. Haas and Chris Jermaine . Describes basic principles and recent developments in approximate query processing. It focuses on four key synopses: random samples, histograms, wavelets, and sketches. It considers issues such as accuracy, space and time efficiency, optimality, practicality, range of applicability, error bounds on query answers, and incremental maintenance. It also discusses the trade-offs between the different synopsis types.

10. [Distributed Streams Algorithms for Sliding Windows](http://home.engineering.iastate.edu/~snt/pubs/tocs04.pdf) by Phillip B. Gibbons and Srikanta Tirthapura 

11. [Frugal Streaming](http://blog.aggregateknowledge.com/2013/09/16/sketch-of-the-day-frugal-streaming/)

12. [A Framework for Clustering Massive-Domain Data Streams](http://charuaggarwal.net/cskrevise.pdf) by Charu C. Aggarwal

13. [A framework for clustering evolving data streams](http://dl.acm.org/citation.cfm?id=1315460) by Charu C. Aggarwal et. al.
 
14. [Unsupervised Feature Selection on Data Streams](https://www0.bnl.gov/isd/documents/89130.pdf) by Hao Huang

15. *Presentations*
  * [Spark Streaming Use Cases](http://www.slideshare.net/pacoid/spark-streaming-case-studies) by Paco Nathan 
  * [Tiny Batches in the wine, Shiny new bits in Spark Streaming](http://www.slideshare.net/pacoid/tiny-batches-in-the-wine-shiny-new-bits-in-spark-streaming) by Paco Nathan
  * [Real time Data Analysis Patterns](http://de.slideshare.net/mikiobraun/realtime-data-analysis-patterns) by Mikio Braun
  * [Streaming Big Data with Apache Spark, Kafka and Cassandra](http://www.slideshare.net/helenaedelson/streaming-big-data-with-apache-spark-apache-kafka-and-apache-cassandra-delivering-meaning-in-nearreal-time-at-high-velocity-at-massive-scale) by Helena Edelson
  * [Streaming Data Analysis and Online Learning](https://www.hakkalabs.co/articles/streaming-data-analysis-and-online-learning/) by John Myles White
  * [Algebra for Analytics](https://speakerdeck.com/johnynek/algebra-for-analytics) by Oscar Boykin @posco

16. *Courses*
  * [Alex Smola course at Berkeley SML: Data Streams](http://alex.smola.org/teaching/berkeley2012/streams.html)
  * [Piotr Indyk course at MIT Sketching, Streaming and Sub-linear Space Algorithms](http://stellar.mit.edu/S/course/6/fa07/6.895/)
  * [Andrew McGregor course at UMass on Advanced Algorithms](http://people.cs.umass.edu/~mcgregor/courses/CS711S12/index.html)
  * [Amit Chakrabarti course at Dartmouth on Data Stream Algorithms](http://www.cs.dartmouth.edu/~ac/Teach/CS49-Fall11/) and the entire course notes in [a single document](http://www.cs.dartmouth.edu/~ac/Teach/CS49-Fall11/Notes/lecnotes.pdf)

17. *Incremental Learning with Decision Trees for Streamed Data*
  * [Mining High-Speed Data Streams (Hoeffding Trees)](http://homes.cs.washington.edu/~pedrod/papers/kdd00.pdf) by Pedro Domingos and Geoff Hulten
  * [Mining Time Changing Data Streams](http://homes.cs.washington.edu/~pedrod/papers/kdd01b.pdf) by G. Hulten, L. Spencer, and P. Domingos.
  * [Comprehensive study on techniques of Incremental learning with decision trees for streamed data](http://www.ijeat.org/attachments/File/V1Issue3/C0201021312.pdf) by Prerana Gupta, Amit Thakkar, Amit Ganatra
  * [Use of Hoeffding trees in concept based data stream mining](http://ieeexplore.ieee.org/xpl/articleDetails.jsp?arnumber=4544780) by Hoeglinger, S. and Pears, R.
  
18. *Clustering Data Streams*
  * [Clustering Data Streams: Theory and Practice](http://infolab.stanford.edu/~loc/tkdepaper.pdf) by Sudipto Guha, Adam Meyerson, Nina Mishra, Rajeev Motwani and Liadan O’Callaghan 
  * [Online clustering of data streams](http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.83.728) by J. Beringer, E. Hüllermeier
  * [Conquering the divide: Continuous clustering of distributed data streams (2007)](http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.131.5316) by Graham Cormode
  * [Clustering on Streams](http://www.cs.utah.edu/~suresh/papers/enc-db/entry.pdf) by Suresh Venkat
 
