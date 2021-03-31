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
