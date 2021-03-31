# Spark NLP Section02 - Soumya Chidambar Rao Waddankeri

%md

# Spark NLP - Soumya Chidambar Rao Waddankeri

> Using PySpark Natural Language Processing 

- Cleaning 
- Processing
- Charting 

## Cleaning
 - NLP Stopword removal
 - remove all non-letters
 
## Processing
 
 - Flatmap from one to many (one line of text to many words)
   - cast everything to lowercase
   - strip whitespace from beginning and end
   - split by our delimiter (space,comma)
 - map() into intermediate key-value pairs
 - filter() to get just some records
 - reduceByKey() to get the count

## Charting

---------------------------
# Spark RDD map reduce exercise

# RDD = resilient, distributed dataset
# Spark  has transofrmations(e.g.,map(), filter(), reduceByKey()) and actions (e.g., collect())
# Make a python list

words = ["one","fish","two","fish","red","fish","blue","fish"]

# create a spark RDD using the spark context object sc
nservers=  4
sc.parallelize(words,nservers)
print(type(rddData))
rddIntermediateKVPairs = rddData.map(lambda w:(w,1))
print(rddIntermediateKVPairs.collect()

