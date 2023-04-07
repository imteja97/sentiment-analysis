# sentiment-analysis
Hey everyone! Today, we'll be working with the IMDB movie reviews dataset to predict sentiments - either positive or negative. Understanding customer sentiment is crucial for businesses to improve their products and services.
1. Importing Libraries: Firstly, we start off by downloading packages word cloud and Nltk which are provided with a range of tools to perform text analysis. Furthermore, we also import necessary libraries numpy, pandas, matplotlib, seaboarn and machine learning libraries. 
2. Data Exploration: We start by loading the dataset, saving it in a dataframe and exploring its structure, like the shape and information of the dataset. We also check the distribution of sentiments and display some sample reviews to get a better understanding of our data. The sentiment distribution plot depicts the distribution of both the positive and negative reviews and it is understood that both the classes are balanced. Also, from the reviews it is quite evident that the reviews contains a lot of special characters. 
3. Preprocessing: A function is written which counts the number of words in the review column and creates a new column in the data frame to show the same. All the sentences in the review column is converted to lower case using the function str.lower() and is necessary to maintain the consistency of the dataset, and as well normalize it. We also encode the sentiment column containing positive and negative to 1’s and 0’s respectively so that the ML model understands it better. Other, preprocessing techniques include below.
* Removing HTML tags, special characters. 
* Stopwords
* Stemming words
* Removing duplicate entries
4. Visualizations- The frequency of different words in both positive and negative reviews is checked using the Wordcloud library and is plotted using matplotlib. 
5. Splitting and feature engineering- The dataset is split into test and train sets where review column is selected as X and Y(outcome) is selected as sentiment. Test size is set to 30%. TF-IDF is used to convert raw text data to numerical features which is important for machine learning models to make predictions. 
6.  Modelling and Evaluation: Now we apply different classification models. 
7. Logistic Regression- Logistic regression is a statistical model used for binary classification tasks, where the goal is to predict one of the two possible outcomes based on the input. 
8.  Multinomial Naive Bayes- The idea behind the Naive bases theorem is to predict the outcome of each class based on the words in a text. 
9.  Decision Tree Classifier.- The idea behind DT is that the input data is recursively split into subsets based on the input values. We evaluate their performance using accuracy, classification reports, and confusion matrices.
10. Discussing Models: Logistic Regression performs well on this dataset, providing a good balance between precision and recall. The Multinomial Naive Bayes model, while less accurate, is faster to train and can still provide decent results. The Decision Tree Classifier tends to overfit and might not generalize well to unseen data.
11. Gotchas and Challenges
In sentiment analysis, some challenges include understanding nuances in the text, dealing with sarcasm or irony, and detecting negation. More advanced models like BERT or GPT have achieved over 90% accuracy on similar datasets.
