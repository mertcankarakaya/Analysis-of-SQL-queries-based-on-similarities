# Analysis of SQL queries based on similarities

## The Project of Goal

The Graduating Project we completed with a team of two includes analysis of SQL Queries with Text Mining.

## Project Process

>**Data Processing**

We accepted thousands of SQL query strings, which we wrote and which were found from certain sources, as Text. 
And applied '[Data Processing](https://github.com/mertcankarakaya/Analysis-of-SQL-queries-based-on-similarities/blob/master/asil_onisleme.py)' to these Textual data.

![clean data](image/1clean_data.png)


>**NLP Approaches and Clustering**

The data were converted into numerical data with [Bag of Words (BoW)](https://github.com/mertcankarakaya/Analysis-of-SQL-queries-based-on-similarities/blob/master/bow_kume_bilgi.py) and [TF-IDF](https://github.com/mertcankarakaya/Analysis-of-SQL-queries-based-on-similarities/blob/master/tfidf_kume_bilgi.py), which is one of the Natural Language Processing methods.
Clustering was carried out by [k-Means algorithm](https://github.com/mertcankarakaya/Analysis-of-SQL-queries-based-on-similarities/blob/master/kumeleme.py) of Machine Learning. 

![numerical data](image/2numerical_data.png)

![clustered data](image/3clustered_data.png)

>**Cluster number decision**

It was deemed appropriate to divide it into 5 clusters using the [WCSS (In-Squares Total)](https://github.com/mertcankarakaya/Analysis-of-SQL-queries-based-on-similarities/blob/master/wcss_hesaplama.py) method.

![wcss](image/4wcss.png)



>**Result**

In order to understand that clusters are separated according to their similarities, each cluster is visualized and analyzed with Power BI. 
As a result, the values within each cluster are different.

[Power BI](https://github.com/mertcankarakaya/Analysis-of-SQL-queries-based-on-similarities/blob/master/thesis_project.pbix) results obtained are shown below.

***Result of Power BI***

![bow cluster](image/bow_cluster.png)

*BoW Cluster chart*

![tfidf cluster](image/tfidf_cluster.png)

*TF-IDF Cluster chart*

![most table](image/most_word2.png)
![most table2](image/4_most_word.png)

*Most worlds*
