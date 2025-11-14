**E-Commerce Customer Review Analysis & Recommendation Engine**

A full ETL + NLP + Topic Modeling + Recommendation Pipeline using SQL, MongoDB, VADER, LDA & Machine Learning

**Overview**

This project simulates the backend infrastructure of a modern e-commerce analytics system.
It integrates structured SQL data (Users, Products, Orders) with unstructured MongoDB data (Customer Reviews & User Logs).

The goal is to build an end-to-end ETL + EDA + NLP + ML workflow capable of:

-> Creating and populating SQL and MongoDB databases

-> Performing sentiment analysis with VADER

-> Conducting topic modeling using LDA (Latent Dirichlet Allocation)

-> Visualizing sentiment distributions

-> Merging relational + NoSQL data

-> Building a =product-category recommendation model

**Technologies Used**

**Databases**

SQLite (Structured Data)

MongoDB Atlas (Unstructured Data)

**Python Libraries**

sqlite3

pymongo

faker

nltk (VADER, stopwords, lemmatization)

matplotlib, seaborn

pandas

gensim (LDA)

pyLDAvis

sklearn (Naive Bayes classifier)

**Dataset Description**

**SQL Structured**


| Table        | Description                                      |
| ------------ | ------------------------------------------------ |
| **Users**    | User details with region                         |
| **Products** | Product catalog with category & pricing          |
| **Orders**   | Transaction history with amount, quantity, dates |

**MongoDB Unstructured**

| Collection    | Description                                    |
| ------------- | ---------------------------------------------- |
| **reviews**   | Customer reviews, ratings, and timestamps      |
| **user_logs** | Behavioral logs: views, add-to-cart, purchases |

**Features Implemented**

**Structured Database Creation (SQLite)**

Auto-generated Users

Auto-generated Products

50 synthetic orders with timestamps and totals

**Unstructured Database Creation (MongoDB)**

Inserts random reviews using Faker

Inserts 100 user activity logs

**Sentiment Analysis (VADER)**

Computes:

Compound score

POS/NEG/NEU polarity

Saves results back to MongoDB

**Data Merging & EDA**

SQL + MongoDB merged on product_id and user_id

Category-wise sentiment distribution charts

Product-wise sentiment distribution charts

**Topic Modeling (LDA)**

Text cleaning (tokenization, lemmatization, stopword removal)

Gensim LDA model

WordClouds

Dominant topic assignment

**Machine Learning Recommendation Engine**

Predicts which product category to recommend using:

Ratings

Sentiment score

Model used: Gaussian Naive Bayes (lightweight & interpretable).

**Project Structure**

├── README.md

├── FinalProject_code.ipynb (or .py)

├── sql_data (in-memory)

└── MongoDB Atlas cluster

wordcloud

This project is suitable for academic submissions, portfolio demonstrations, and learning hybrid database analytics.
