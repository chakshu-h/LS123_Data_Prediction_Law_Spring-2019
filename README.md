# Legal Studies 123: Data, Prediction, and Law

This repository contains the course materials for Legal Studies 123: Data, Prediction and Law offered at UC Berkeley during Spring 2019.

## Table of Contents

1. [Introduction](https://github.com/Akesari12/LS190#Introduction)
2. [Course Goals](https://github.com/Akesari12/LS190#Course-Goals)
3. [Social Science Data](https://github.com/Akesari12/LS190#Social-Science-Data)
4. [Machine Learning & Policing](https://github.com/Akesari12/LS190#Machine-Learning-&-Policing)
5. [Law as Text as Data](https://github.com/Akesari12/LS190#Law-as-Text-as-Data)
6. [Lab Plan](https://github.com/Akesari12/LS190#Lab-Plan)
7. [Conclusion](https://github.com/Akesari12/LS190#Conclusion)

## Introduction

The course is aimed at an undergraduate audience, and allows students to explore different data sources that scholars and government officials use to make generalizations and predictions in the realm of law. The course also introduces critiques of predictive techniques in law. Students  apply the statistical and Python programming skills to examine a traditional social science dataset, “big data” related to law, and legal text data. The materials here will enable anyone who is interested in teaching a similar course to do so with minimal additional preparation.

The course was developed in cooperation with UC Berkeley's Data Science Education Program (DSEP). DSEP provided critical support in the form of a seed grant, and developing most of the notebooks that we used for in-class lab sessions. As such, this course is geared towards students who completed Berkeley's Data 8: Foundations of Data Science course. Data 8 introduces computational and inferential thinking, and encourages students to apply it to real-world data and problems. Topics include basic probability, hypothesis testing, regression and classification, and computation in Python.

## Course Goals

## Social Science Data

The first unit of the course exposes students to traditional social science data, refreshes programming concepts from Data 8, and exposes students to some introductory readings and concepts that integrate Big Data and social science. We start with covering more traditional social science topics because they provide a gentle introduction to statistical concepts such as hypothesis testing and probability, and help motivate why data science opens up new opportunities in the social sciences. 

One main goal in this unit is to help students distinguish between causation and prediction in the social sciences. For students coming from more traditional social science backgrounds, techniques such as regression were likely taught as tools for uncovering causal estimates. This course instead aims to explore the relationship between prediction and law, and therefore give students a strong intuition over what it means to develop a predictive algoirthm instead of a causal model. Both prediction and causation still rely on fundamental statistical concepts such as probability, hypothesis testing, and regression, so we cover these with an eye toward explaining how they relate to specific legal problems.

## Big Data & Policing

After reviewing the basics of social science and statistics, we move to integrating big data into the study of law. Many of our examples were drawn from criminal justice as this is a major subfield within law, and provides ample sources of publicly available data. Crime also brings forward some of the most salient debates in law and algorithms, particularly with regards to using algorithms for predictive policing, probation, and sentencing. In this unit, we assigned readings such as Kleinberg et. al.'s "Human Predictions and Machine Decisions" and ProPublica's investigation into Broward County's use of the COMPAS algorithm. 

Our main substantive goal was to help students realize that crime, and by extension most other legal and social pheonomena, follow particular patterns that oftentimes break down along racial, gender, and income lines. We challenged students to think about ways to engage in policing, auditing, and other regulatory behaviors without taking this sort of information into account. Ultimately, we wanted students to leave with an understanding that simply leaving something like "race" out of a training set does not guarantee a substantively fair outcome.

On the technical side, we focus on teaching students basic geographic information systems (GIS) and machine learning techniques in Python. For GIS techniques, we primarily taught students how to use the folium package. Folium is a useful GIS implementation because it allows students to deal with many different data structures and layer them. It also allows students to create interactive maps, and thus exposes them to some elements of software design. We also introduce students to geopandas as a tool for manipulating geospatial data structures. We then had students deploy GIS techniques to visualize crime in Berkeley and San Francisco. Visualizing crime in Berkeley was especially illuminating because the students could see how crime was distributed in their own neighborhoods. We encouraged students to think about how police departments prioritize which neighborhoods to patrol based on this spatial distribution, and critique the ethics of this kind activity. 

We then move to introducing machine learning models and relating them to predictive policing. On the technical side, we use Introduction to Statistical Learning to introduce students to the basics of developing machine learning models. Here, we distinguish between regression and classification problems, and guide students through developing models through training and test sets. We also introduce concepts such as cross-validation, regularization, and other tools for tuning machine learning models. 

As a whole, our goal with this unit was to provide students with both the technical skills to develop their own maps and machine learning models, while also making them cognizant of how things like crime intersect with race, gender, income, and other societal factors. Beyond crime, we want students to realize that simply excluding certain features from an algorithm does not guarantee fairness. We believe that the best way to illustrate this concept is to have students build models themselves and truly grapple with the challenge of creating "fair" algorithms. 

## Law as Text as Data

## Lab Plan

| Lab Date | Summary                                                               | Data                                                   | 
|----------|-----------------------------------------------------------------------|--------------------------------------------------------|
| 1-28-19  | Anaconda Setup                                                        | American National Election Study (ANES)                              | 
| 1-30-19  | Dataframe operations, Scatter Plots, Histograms, Probability          | ANES                                                   | 
| 2-4-19  | Empirical Distributions and Hypothesis Testing                        | ANES                                                   | 
| 2-6-19  | Bootstrap and Confidence Intervals                                    | ANES| 
| 2-11-19 | Regression Models                                                      | ANES| 
| 2-13-19   | Mapping with Folium                                                  | us-states.json, US Unemployment October 2012      | 
| 2-20-19  | Folium: Choropleth Maps                                               | us-states.json, US Unemployment October 2012      | 
| 2-25-19  | Folium: Heat Maps + Time                                              | us-states.json, US Unemployment October 2012      | 
| 2-27-19  | Folium Plugins                                                        | us-states.json, US Unemployment October 2012  | 
| 3-4-19  | Intro to Numpy/Scipy                                                   | None| 
| 3-6-19  | Intro to Regression and the Test-Train-Validation Split               | Bike Sharing                                       | 
| 3-11-19  | Model Selection and Cross Validation                                  | Bike Sharing                                      | 
| 3-13-19  | Feature Selection                                                     | Bike Sharing                                      | 
| 3-18-10   | Text Preprocessing : Stemming, Chunking, Tokenizing                   | UN General Assembly Transcripts                  | 
| 3-20-19  | Exploratory Data Analysis                                             | | 
| 4-1-19   | Introduction to Text Analysis : Document-Term Matrix                  | UN General Assembly Transcript                    | 
| 4-3-19  | Web Scraping and XML Parsing                                          | Old Bailey Online Corpus                           | 
| 4-8-19  | Regular Expressions                                                   | Old Bailey Online Corpus                           | 
| 4-10-19  | TF-IDF and Classification: Naive Bayes, Multinomial Logistic, SVM     | Stack Exchange Queries                            | 
| 4-15-19  | Exploratory Data Analysis: Feature Extraction, Visualizations, PCA    | 2016 US Presidential Campaign Speeches            | 
| 4-17-19   | Neural Nets: Multi-Layered Perceptron, Convolutional Neural Netowkrs  | MNIST                                                  | 
| 4-22-19   | Word2Vec and Word Embeddings                                          | UN General Debate Transcripts                          | 
| 4-24-19  | Topic Modeling: Latent Dirichlet Analysis in Gensim and Scikit-learn  | UN General Debate Transcripts                          | 
| 4-29-19  | Text Analysis: Sentiment, Morality, Non-Negative Matrix Factorization | Old Bailey Online Corpus                               | 
| 5-1-19  | Decision Trees and Ensemble Methods                                   | Bike Sharing                                           | 

## Conclusion
