# Sentiment-Analysis-of-COVID-19-Tweets

<h2>Overview</h2>

This project focuses on sentiment analysis using machine learning techniques to classify tweets into sentiment categories. The dataset used contains tweets related to various topics, and the goal is to predict sentiment labels for these tweets.

<h2>Dataset</h2>

The dataset (Corona_NLP_train.csv) consists of the following columns:

1. UserName: ID of the user
2. ScreenName: ID of the user's screen name
3. Location: Location of the user
4. TweetAt: Date of the tweet
5. OriginalTweet: Text content of the tweet
6. Sentiment: Sentiment label (Positive, Negative, Neutral, Extremely Positive, Extremely Negative)

<h2>Data Preprocessing</h2>

Data cleaning: Removing URLs, user mentions, and non-alphanumeric characters.

Stopwords removal: Removing common English stopwords using NLTK library.

Lemmatization/Stemming: Reducing words to their base or root form using NLTK's WordNetLemmatizer or PorterStemmer.

<h2>Exploratory Data Analysis (EDA)</h2>

Visualization of sentiment distribution using bar plots and pie charts.

Analysis of tweet frequencies over time using line plots and histograms.

<h2>Feature Engineering</h2>

1. Vectorization: Converting text data into numerical form using Count Vectorization.
  
2. Feature selection: Selecting relevant features or words that contribute to sentiment classification.
   
<h2>Model Training</h2>

Implemented multiple machine learning models including:

1. Stochastic Gradient Descent (SGD)
2. Logistic Regression
3. CatBoost
4. Support Vector Machines (SVM)
5. Random Forest
6. Naive Bayes

**Models were trained and evaluated for both multiclass and binary sentiment classification tasks.**

<h2>Model Evaluation</h2>

Evaluation metrics used: Accuracy score, classification report (precision, recall, F1-score), confusion matrix.

**Results**

**1. Multiclass Sentiment Classification**

1. CatBoost: 62.32%
2. Logistic Regression: 61.36%
3. SVM: 60.79%
4. SGD: 56.39%
5. Random Forest: 56.29%
6. Naive Bayes: 46.87%

**2. Binary Sentiment Classification**
1. SGD: 85.73%
2. Logistic Regression: 85.54%
3. CatBoost: 84.69%
4. SVM: 83.95%
5. Random Forest: 81.98%
6, Naive Bayes: 77.59%

<h2>Conclusion</h2>

**Multiclass Classification:** CatBoost performed best, followed by Logistic Regression and SVM.

**Binary Classification:** SGD and Logistic Regression excelled, closely followed by CatBoost and SVM.
