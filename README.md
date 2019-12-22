# Sentiment Analysis of Tweets

1) I have considered 2000 tweets and retweets from search api. I am extracting full text of each tweet i.e., extended text of the tweet.
2) Performed data cleaning by removing URLs, special characters, emoticons, etc., from the tweets.
3) Created bag-of-words for each tweet and, stored them in a dictionary of tweets as keys and their list of bag-of-words as value.
4) Used Lexicon-Opinion list of words(attached to the repository) to identify the polarity of the tweets. Two files namely 
‘negative-words.txt’ and ‘positive-words.txt’ are used.
5) In each tweet, based on the count of positive and negative number of words, polarity has been decided. If the count of negative words 
in the tweet is more than that of positive words, the polarity of the tweet is tagged as ‘NEGATIVE’. If the count of positive words in the
tweet is more than that of negative words, the polarity of the tweet is tagged as ‘POSITIVE. If both the counts are equal, the tweet is
tagged as ‘NEUTRAL’.
6) The final data with tweet no, tweet text, list of matched words, polarity has been exported to a csv file named ‘sentiment-output.csv’.

# Semantic analysis of news articles

1) I have extracted the files from ‘reut2-020.sgm’ and ‘reut2-021.sgm’. A total of 1578 files have been 
extracted.
2) Data cleaning has been performed while extracting the files itself, by removing HTML tags, special characters etc. All the files have 
been stored into a folder named ‘articles’ in the same directory.

Part a: 
Now, using the search query “Canada”, “Halifax”, “Nova Scotia”, and searching in how many documents these words have appeared.

<ul>
<li>
Looped through all the 1578 files that are in the articles folder and searched for the words “Canada”, “Halifax”, “Nova Scotia” to find 
out the count of number of documents these words have appeared. The word “Canada” has been appeared in total of 27 files whereas “Halifax”
and “Nova Scotia” are not found.
</li>
<li>
The output has been printed in the .ipynb file with the columns, search word, number of documents containing the search word, total 
number of documents/number of documents search word appeared, Log10(N/df).
</li>
<li>
Also, the output has been exported to csv file named ‘semantic_output_part_a.csv’.
</li>
<li>
Since the ‘Halifax’ and ‘Nova Scotia’ have not appeared in any of the 1578 documents, the Log10(N/df) has been printed as ‘N/A’
</li>
</ul>
<p>
The output can be seen here.. 
</p>
<a href="https://ibb.co/6Rjjrjb"><img src="https://i.ibb.co/FbRRmRJ/1.png" alt="1" border="0"></a>


Part b:
Using the above table, we need to find which document has the highest occurrence of the word “Canada”. We can find this by performing 
frequency count of the word per document.

<ul>
<li>
In this step, number of times the word “Canada” is repeated in each document is calculated and is printed to a table with columns, file 
name, total number of words in that file, frequency of the word “Canada” and, Relative frequency.
</li>
<li>
To find out the count, I have searched for all the words including the upper, lower and other kind of cases in each document.
</li>
<li>
Along with printing it in the ipynb file, the resultant table has also been exported to csv file named ‘semantic_output_part_b.csv’.
</li>
<li>
The document which has the highest occurrence of the word “Canada” has been identified.
</li>
</ul>
<p>
The output can be seen here..  
</p>
<a href="https://ibb.co/ZgRdMbj"><img src="https://i.ibb.co/7pxv10f/2.png" alt="2" border="0"></a>

Part c:
Finally, the news article which has the highest relative frequency(f/m) has been identified and is printed in the ipynb file.
<p>
The output can be seen here..  
</p>
<a href="https://ibb.co/cbVWk91"><img src="https://i.ibb.co/1sjC7NL/3.png" alt="3" border="0"></a>


All the above-mentioned output files have been attached to the repository for reference.
