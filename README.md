Stanford-Sentiment-Analyzer
===========================

This code is released by Stanford for Sentiment Analysis.

The jar files required to run this code are as follows:

    
ejml-0.23.jar
javax.json.jar
javax.json-api-1.0-sources.jar
joda-time.jar
joda-time-2.1-sources.jar
jollyday.jar
jollyday-0.4.7-sources.jar
xom.jar
xom-1.2.10-src.ar

I am not sure if all of these jar files are essential or not. I had all of these imported, so I mentioned all of them.

How to run this code
--------------------

I navigate to src/edu/stanford/nlp/sentiment
Then I run:
java -cp stanford-corenlp-3.4.jar:stanford-corenlp-3.4-models.jar:xom.jar:joda-time.jar:jollyday.jar:ejml-0.23.jar -mx5g edu.stanford.nlp.sentiment.SentimentPipeline -file input.txt
(If I have the input in a file)
or
java -cp stanford-corenlp-3.4.jar:stanford-corenlp-3.4-models.jar:xom.jar:joda-time.jar:jollyday.jar:ejml-0.23.jar -mx5g edu.stanford.nlp.sentiment.SentimentPipeline -stdin
(If I want to give input line by line)

If I want the output in tree form, I add -output PENNTREES as an argument to the above-mentioned command
