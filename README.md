COMPANY: CODTECH IT SOLUTIONS

NAME: ARYA DILIP BHONGALE

INTERN ID:CTIS4921

DOMAIN:MACHINE LEARNING

DURATION:4 WEEKS

MENTOR:NEELA SANTHOSH KUMAR

DESCRIPTION-
This project aims to perform Sentiment Analysis on the Amazon Fine Food Reviews dataset using Natural Language Processing (NLP) techniques and a supervised machine learning algorithm. Sentiment analysis is a branch of text mining that focuses on identifying and classifying opinions expressed in textual data. In the context of e-commerce, customer reviews contain valuable insights about product quality, user satisfaction, and overall experience. Manually analyzing thousands of such reviews is impractical; therefore, automated sentiment classification systems are essential.

The dataset used in this project consists of customer reviews along with additional metadata such as product identifiers, user identifiers, helpfulness scores, ratings, and timestamps. For the purpose of sentiment analysis, the primary features utilized were the “Text” column, which contains the full review content, and the “Score” column, which represents the rating given by the customer on a scale of 1 to 5. To convert the rating into sentiment labels, ratings of 1 and 2 were categorized as negative sentiment, ratings of 4 and 5 were categorized as positive sentiment, and rating 3 was treated as neutral and removed to simplify the problem into binary classification. This transformation allowed the model to learn clear distinctions between positive and negative opinions.

Before applying machine learning techniques, the textual data underwent preprocessing. Text preprocessing is a crucial step in NLP because raw text often contains noise such as punctuation marks, special characters, inconsistent capitalization, and extra spaces. The preprocessing steps included converting all text to lowercase to ensure uniformity, removing non-alphabetic characters using regular expressions, and eliminating unnecessary whitespace. These steps improve the quality of input data and help the model focus on meaningful textual patterns rather than irrelevant symbols.

Since machine learning algorithms cannot directly interpret raw textual data, feature extraction was performed using TF-IDF (Term Frequency–Inverse Document Frequency) vectorization. TF-IDF is a statistical technique used to evaluate the importance of a word in a document relative to a collection of documents. Term Frequency (TF) measures how frequently a word appears in a specific document, while Inverse Document Frequency (IDF) reduces the weight of words that appear frequently across many documents. By multiplying TF and IDF, the method assigns higher weights to words that are distinctive and meaningful within a review. This process converts textual data into numerical vectors, enabling mathematical computation and model training.

After vectorization, Logistic Regression was employed as the classification algorithm. Logistic Regression is a supervised learning technique widely used for binary classification tasks. Unlike linear regression, which predicts continuous values, logistic regression predicts probabilities using the sigmoid function. The sigmoid function maps any real-valued input into a range between 0 and 1, which represents the probability of belonging to a particular class. Based on a threshold value (commonly 0.5), the model assigns the review to either positive or negative sentiment. Logistic Regression was chosen due to its simplicity, efficiency, interpretability, and strong performance in text classification problems.

The dataset was divided into training and testing sets to evaluate model performance effectively. The model was trained on the training data and evaluated on unseen test data. Several evaluation metrics were used to assess performance, including accuracy score, classification report (which provides precision, recall, and F1-score), and confusion matrix. Accuracy measures the overall correctness of predictions, while precision and recall provide deeper insights into the model’s ability to correctly classify positive and negative reviews. The confusion matrix visually represents correct and incorrect predictions, helping to identify potential classification errors.

In addition to model evaluation, data visualization techniques were applied to gain insights into the dataset. Visualizations included rating distribution, sentiment distribution, review length analysis, and graphical representation of the confusion matrix. These visual tools help in understanding data imbalance, text characteristics, and model effectiveness.

The results demonstrate that TF-IDF combined with Logistic Regression can effectively classify customer reviews with high accuracy. However, performance may be influenced by class imbalance and feature selection parameters. Future improvements may include hyperparameter tuning, incorporating n-grams, handling imbalance using resampling techniques, or applying advanced deep learning models such as LSTM or transformer-based architectures.

In conclusion, this project successfully demonstrates how Natural Language Processing and machine learning techniques can be integrated to build an automated sentiment analysis system. Such systems have significant real-world applications in e-commerce, marketing analytics, customer service optimization, and brand monitoring. By leveraging textual data effectively, businesses can make informed decisions based on customer feedback and improve overall product quality and user satisfaction.
