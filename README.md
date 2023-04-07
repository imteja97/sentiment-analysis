# sentiment-analysis
Importing Libraries: We first import necessary libraries like pandas, numpy, seaborn, and various machine learning models.

Loading Data: We load the IMDB Dataset.csv, which contains movie reviews and their sentiments (positive or negative).

Exploring Data: We check the shape, information, and distribution of sentiments. We also display the first five reviews to understand the data better.

Preprocessing Data: We preprocess the reviews by converting them to lowercase, removing HTML tags, special characters, and stopwords, as well as stemming the words. We also remove duplicate entries.

Visualizations: We create word clouds for positive and negative reviews to get a visual representation of frequently used words in both types of reviews.

Splitting Data: We split the data into training and testing sets, which will be used to train and evaluate the machine learning models.

Feature Engineering: We use the TfidfVectorizer to convert the text data into numerical features that can be used by machine learning models.

Modelling and Evaluation: We apply different machine learning models (Logistic Regression, Multinomial Naive Bayes, and Decision Tree Classifier) and evaluate their performance using accuracy, classification reports, and confusion matrices.
