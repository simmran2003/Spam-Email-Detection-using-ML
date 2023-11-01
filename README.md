# Spam-Email-Detection-using-ML

**OVERVIEW**:
What is an E-mail spam filter?
An email spam filter is a tool used in email hosting software that churns out unsolicited, unwanted, and virus-infected emails and keeps such emails off of the user’s inbox. This protects the user from any potential cyber threat and facilitates smooth communications and workflow.
Why is a spam filter necessary?
The security risk can be reduced since the user gets in hand the emails that have gone through various spam checks. Moreover, these email spam filters throw out malware, malicious, and virus-infected emails and protect user security.
Spam emails pose a significant threat to email users, leading to increased clutter, security risks, and potential financial losses. To combat this issue, machine learning techniques, such as logistic regression, have proven to be effective in identifying and filtering out spam emails. This report discusses the application of logistic regression for spam email detection, outlining the methodology, data preprocessing, model training, evaluation, and future recommendations.

**METHODOLOGY**:
1. **Data Collection**
The success of a spam email detection system largely depends on the quality and quantity of data available. A dataset containing a diverse range of spam and non-spam (ham) emails is essential. Commonly used datasets include the SpamAssassin Public Corpus and the Enron Email Dataset.
2. **Data Preprocessing**
Data preprocessing plays a crucial role in preparing the dataset for modeling. This includes:
-	**Text Cleaning**: Removing special characters and irrelevant whitespaces.
-	**Tokenization**: Splitting the text into words or tokens.
-	**Feature Extraction**: Converting text into numerical features, typically using techniques like TF-IDF
(Term Frequency-Inverse Document Frequency)
3. **Model Selection**
Logistic regression is a suitable choice for binary classification problems like spam detection. It models the probability of an email being spam or ham based on the extracted features.
4. **Model Training**
The dataset is split into a training set and a testing set to train and evaluate the logistic regression model. The model is trained using the training data, adjusting its coefficients to minimize the logistic loss function.
5. **Model Evaluation**
To assess the model's performance, various metrics can be used, including:
-	**Accuracy**: The percentage of correctly classified emails.
-	**Precision**: The ratio of true positives to the total predicted positives.
Logistic regression is a robust and interpretable machine learning algorithm for spam email detection. When combined with appropriate data preprocessing techniques and hyperparameter tuning, it can yield high accuracy and help reduce the impact of spam on email users.

**Explanation Of the Code**:
Data is loaded using pandas.
The missing values are replaced by null string.
Emails are marked as Spam and Ham with values of Spam being 0 and Ham being 1
since, we are using logistic regression model, therefore,m a graph needs to be plotted for that we have seperated the data as texts and labels. On the X-axis we have the message and on the Y-axis we have the category.
Dataset is split into training data and test data.Of which 20% is the test data.
We then transform the text data to feature vectors which are used as an input to our logistic regression model.
It is important we covert the Y data to integers as the model works best on int values.
The model is then trained by simply importing the logistic regression library from sklearn.linear_model
we can then check the accuracy of the model, this can be done by creating an accuracy checker for both test and training data.
The model is put to use andmails can now be classified as ham or spam.
A heatmap is then plotted for the same showing which sender sends most spam mails.


