# NLP on Amazon Book Reviews

For my final project at Nod Coding Bootcamp (January-March 2023) I performed some natural language processing and sentiment analysis on textual book reviews from Amazon.  The dataset I used is from Kaggle.com. This project had two parts:  a predictive machine learning model and an exploratory sentiment analysis using existing models. 

For my machine learning model  I chose to focus on building a two-class classification model, so I first removed the star ratings of 3, then the 1 and 2 star ratings became classified as negative (0) and the 4 and 5 star ratings became classified as positive (1).  I then took a random sample of 100,000 reviews, though I made sure to balance the actual classes equally to avoid having imbalance.  After training my data on a few different models I chose to use NaiveBayes-Multinomial.  Upon running my test data through this model, I achieved 87.4% accuracy in predicting whether a review had a postive or negative rating, based only on the review text.  What I learned from this project was the importance of preprocessing the text data, which was the most time-consuming part of the project.  In addition to basic text cleaning, I lemmatized my text to make the model more efficient, and I tested out different n-grams settings for optimal performance.  

The second part of my project was running my sample data through some existing models for sentiment analysis and performing a simple EDA on the results.  I used the VADER and ROBERTA models, and performed a comparison of how each model performed in capturing the sentiment of the review based on the text.

The code for this project is captured in the accompanying files, and the presentation file goes into more detail about my process. 
