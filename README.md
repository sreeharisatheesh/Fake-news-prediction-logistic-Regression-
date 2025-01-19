
# Fake News Detection

This project implements a Fake News Detection system using machine learning in Python. It utilizes the Kaggle Fake News Dataset to classify news articles as either real or fake based on their content. The system employs a Logistic Regression model and various preprocessing techniques to achieve high accuracy.

Dataset
Source: Kaggle Fake News Dataset
Files Used: [train.csv](https://www.kaggle.com/c/fake-news/data?select=train.csv)



Project Workflow



1. Preprocessing
Handled missing values by:
Dropping columns with many missing values.
Dropping rows with missing entries.
Combined the author and title columns into a single feature (content).
Applied stemming to reduce words to their root forms.
Removed stopwords (e.g., "a", "the") for better feature extraction.
Converted text into numerical features using TF-IDF Vectorization.



2. Splitting the Dataset
Split the processed dataset into training and testing sets using an 80-20 ratio.
3. Model Selection
Used Logistic Regression to classify news articles.
Evaluated the model using accuracy score to measure performance.
4. Prediction
The model predicts whether a given article is real or fake based on the trained Logistic Regression classifier.



Dependencies
The project requires the following Python libraries:

pandas: For data manipulation.
numpy: For numerical operations.
nltk: For text preprocessing, including stopwords and stemming.
scikit-learn: For machine learning tasks, including feature extraction, model building, and evaluation.



Install the dependencies using:

```bash
pip install pandas numpy nltk scikit-learn
```
