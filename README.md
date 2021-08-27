# Text-matching-System-for-Question-Matching

## Abstract
Building a Text matching system has a high practical significance for retrieving relevant text from a large number of documents. Three different methods namely TFIDF, word average embedding method and inverse document frequency method were used to build a text matching system. The systems were tested on the first 100 questions which were duplicate. A maximum accuracy score of 77% and 67% in top5 and top 2 matches was obtained using average word model.

## Introduction
Text matching is a part of Natural Language Processing (NLP). NLP helps computers read, understand and interpret human language. It is being widely used for sentiment analysis, language translation, text extraction, chatbots etc. With the increasing number of online platforms containing comments, reviews, question and answer forums etc., the task of matching different texts has high practical significance. It can be used to find a similar document or to find the answer to a question. Three different types of algorithms are used to perform text matching. TF-IDF is a simple yet efficient method to perform text matching. It uses a term document matrix. The other two methods, word average and smooth inverse frequency use pretrained word embeddings to create sentence embedding.

## Dataset
The dataset used for this project is a collection of questions. The data is a tsv file named “data.csv” which contains six columns namely, Id, qid1, qid2, question1, question2 and is_duplicate. The column is_duplicate indicates if question 1 and question are duplicate or same. It has two values, 0 and 1. There are 363181 and 363180 questions in question 1 and question 2 respectively. After removing duplicated questions, the class distribution of label observed is shown in Figure 1. There are 63108 reviews labelled as duplicate, 169095 as not duplicate. The classes 0 and 1 are not balanced in the dataset with more than half samples labelled as 1. For training, the questions in question 2 are used. The first 100 questions where is_duplicate is equal to 1 are used for testing. Text matching scores are calculated for each question 1 in the testing test against all questions in question 2. Different evaluation metrics are used for different techniques which are discussed later on in this report.

Further details about this project are avaialable in the report.
