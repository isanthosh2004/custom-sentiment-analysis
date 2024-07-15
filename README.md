## Custom Twitter Sentiment Analysis

Welcome to the Custom Twitter Sentiment Analysis project! This project aims to classify the sentiment of tweets as either positive or negative based on our input tweet using machine learning techniques.

### Features

- Sentiment classification using Logistic Regression.
- Preprocessing of tweets including handling emojis and stopwords.
- Visualization of word clouds for negative and positive tweets.
- Performance evaluation using confusion matrices and classification reports.




### Dataset

- The dataset used is `dataset.csv`.
- The dataset contains the following columns: `sentiment`, `ids`, `date`, `flag`, `user`, `text`.
- Encoding: `ISO-8859-1` (includes almost all Western languages).

### Data Preprocessing

1. **Sentiment Values Replacement**:
    - Replace sentiment value `4` with `1` for positive sentiment.
  
2. **Handling Emojis and Stopwords**:
    - Convert emojis to their respective text meanings.
    - Remove stopwords from the tweets.

3. **Text Cleaning**:
    - Convert text to lowercase.
    - Replace URLs with a placeholder.
    - Replace user mentions with a placeholder.
    - Remove non-alphanumeric characters.
    - Replace consecutive repeating characters with two characters.

### Data Visualization

- **Distribution of Sentiments**:
    - Bar plot showing the distribution of positive and negative sentiments.
  
- **Word Clouds**:
    - Word clouds for the most frequent words in negative and positive tweets.

### Model Training

- **TF-IDF Vectorization**:
    - Convert text data into TF-IDF features with n-grams (1,2) and a maximum of 500,000 features.
  
- **Logistic Regression Model**:
    - Train a Logistic Regression model with `C=2` and `max_iter=1000`.

### Model Evaluation

- Evaluate the model using a classification report and confusion matrix.

### Saving and Loading Model

- Save the trained model and vectorizer using pickle.
- Load the saved model and vectorizer for prediction.

### Prediction

- Predict the sentiment of custom input text using the trained model.



### Badges

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![scikit-learn](https://img.shields.io/badge/scikit--learn-0.24.2-orange)
![nltk](https://img.shields.io/badge/nltk-3.6.3-yellow)
![pandas](https://img.shields.io/badge/pandas-1.3.2-green)

---

Feel free to explore and enhance the project! If you have any questions or suggestions, please contact me.
