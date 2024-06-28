# Movie-Recommender-System
A content based movie recommender system using cosine similarity

# Table of Content
* Demo
* Overview
* Motivation
* Data Collection
* Data Cleaning
* Vectorization(Bag of Words)
* Cosine Similarity
# Overview
I have made Movie Recommender System which gave us 5 recommendations based on our Searched movie. This project showcases my skills on Python, Pandas, Numpy, Count Vectorizer and Cosine similarity.
# Data Collection
Movie dataset Extracted the Dataset from the Kaggle. Kaggle is an Open source and have a large community also they conduct competitions every month,Kaggle allows users to find and publish data sets, explore and build models in a web-based data-science environment, work with other data scientists and machine learning engineers, and enter competitions to solve data science challenges,Given the thousands of other people also doing them, it is becoming harder and harder for merely working through them to be enough to differentiate you. You'll learn a lot, but it won't make you stand out from your competition.Data scientists of all levels can benefit from the resources and community on Kaggle. Whether you are a beginner, looking to learn new skills and contribute to projects, an advanced data scientist looking for competitions, or somewhere in between, Kaggle is a good place to learn.
# Data Cleaning
Data cleaning is the process of fixing or removing incorrect, corrupted, incorrectly formatted, duplicate, or incomplete data within a dataset. When combining multiple data sources, there are many opportunities for data to be duplicated or mislabeled. If data is incorrect, outcomes and algorithms are unreliable, even though they may look correct. There is no one absolute way to prescribe the exact steps in the data cleaning process because the processes will vary from dataset to dataset. But it is crucial to establish a template for your data cleaning process so you know you are doing it the right way every time.

First Merging two tables(movies and credits tables) into one table on basis of movie title and Remove the unnecessary columns Below features doesn't require because it is not necessary it does not impact too much for the recommendation so we removing the below features from the table
* budget
* homepage
* id
* original_language
* original_title
* popularity
* production_comapny
* production_countries
* release-date(not sure)
Accessing required and important columns are ('movie_id','title','overview','genres','keywords','cast','crew') and Find the NULL values we just remove the null values it has contains only 3 null values and "ast" Library performs a collection of nodes that are linked together based on the grammar of the Python language and applied the "ast" techniques to the genres and keywords columns and access the top 3 cast actor from the cast table and remaining actor was drop and create on the function to get the director name from crew column because there is a lot of workers name is there but we want just director name and remove the whitespace from the columns(Sam Worthington, Sam Johny) sometimes user enter Sam machine get confused that's why removing whitespace and also applied the same function for the director name, movies, caste and keywords columns and Splitting each word in overview columns Adding overview, genres, keywords, cast, and crew added into one table -->"Tag" Column table because of vectorization after merging the content of all data into one column Removing the columns overview, genres, keywords, cast and crew.
# Vectorization
Using Bag of Words Techniques for Vectorization
Text data is used in natural language processing (NLP), which interacts between humans and machines using natural language. Text data helps analyze movie reviews, products using Amazon reviews, etc. But the question that arises here is how to deal with text data when building a machine learning model? Text data is converted to a real-valued vector by various techniques. One such approach is Bag of Words (BoW), which will be discussed in this article. But why do we have to convert the text into a vector? Why can’t we use text data to build a machine learning model? Need for text vectorization Let’s say we have reviews of a product. Text reviews provided by the customers are of different lengths. By converting from text to numbers, we can represent a review by a finite length of the vector. In this way, the length of the vector will be equal for each review, irrespective of the text length. Bag of words is the most trivial representation of text into vectors. Each column of a vector represents a word. The values in each cell of a row show the number of occurrences of a word in a sentence.Vectorizing data into 5000 features and applying stop words it removes the unnecessary word from these column-like -->(Is, am, the, was, a, an).
# How Cosine Similarity works?
Cosine similarity is a metric used to measure how similar the documents are irrespective of their size. Mathematically, it measures the cosine of the angle between two vectors projected in a multi-dimensional space. The cosine similarity is advantageous because even if the two similar documents are far apart by the Euclidean distance (due to the size of the document), chances are they may still be oriented closer together. The smaller the angle, higher the cosine similarity.

# Linkdin Profile
For any queries regarding about this project contact me

[Linkedin Profile](https://www.linkedin.com/in/anil-l-b023631b6/)
