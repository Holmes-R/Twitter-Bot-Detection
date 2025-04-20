# Twitter-Bot-Detection

This project focuses on detecting bot accounts on Twitter using machine learning techniques. By analyzing features extracted from user metadata, it aims to classify whether an account is a bot or a human.


## Dataset

The dataset used is training_data_2_csv_UTF.csv, which contains labeled Twitter account data. The key feature is a binary label bot indicating if an account is a bot (1) or a human (0).

##  How do I detect a bot?
  
-  Some typical characteristics of bots on Twitter include:

    - Many Twitter bots have a relatively recent creation date.
    - Many bot user names contain numbers, which can indicate automatic name generation.
    - The account primarily retweets content, rather than tweeting original content.
    - The account’s tweet frequency is higher than a human user could feasibly achieve.
    - The account may have a high number of followers and also be following a lot of accounts; conversely, some bot accounts are identifiable because they send a lot of tweets but only have a few followers.
    - Many bots tweet the same content as other users at roughly the same time.
    - Short replies to other tweets can also indicate automated behavior.
     There is often no biography, or indeed a photo, associated with bot Twitter accounts.

## Project WorkFlow 

1. Data Preprocessing
  - Loaded the dataset using pandas
  - Dropped unnecessary columns and handled missing values
  - Feature selection was performed to identify the most relevant inputs for classification

2. Train-Test Split
  - The dataset is split into training (80%) and testing (20%) sets using a custom function perform_train_test_split()
  - If modified to 90/10, change the test_size parameter accordingly

3. Machine Learning Model
  Algorithm | Accuracy | Precision | Recall | F1 Score
  Logistic Regression | 0.91 | 0.90 | 0.93 | 0.91
  Decision Tree Classifier | 0.86 | 0.85 | 0.87 | 0.86
  Random Forest Classifier | 0.93 | 0.92 | 0.94 | 0.93
  K-Nearest Neighbors | 0.88 | 0.86 | 0.89 | 0.87
  Gradient Boosting Classifier | 0.94 | 0.93 | 0.95 | 0.94
