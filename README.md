<img width="826" alt="pic number 1 " src="https://github.com/abboudcherine/kal281681/assets/155471357/fd225a85-980f-45af-9b47-1edd6c4ebc37"># kal281681                                         AI machine learning project 

### dataset : SafeComm Digital Security Solutions
### members : 
- cherine Abboud ,289351
- kalkidan Mezgebe ,281681
- Ana Andrijasevic ,285991

# Section 1: Introduction

In this project, we developed a machine learning model for SafeComm Digital Security Solutions to identify fraudulent SMS messages. The prevalence of SMS-based fraud poses significant risks, and our model aims to mitigate these by automatically flagging suspicious messages. We utilized an anonymized dataset provided by a telecom partner, containing a mix of regular and potentially fraudulent SMS messages.

Section 2: Methods

Our approach involved several key steps:
Eda and visulisaton : we conducted a  thorough exploratory data analysis (EDA) to gain insights into the dataset. This includes:
Checking for missing values.
Analyzing the distribution of fraudulent vs. non-fraudulent SMS.
Understanding the nature and variety of SMS texts.
Exploring any patterns or trends over time (based on the 'Date and Time' column).

<img width="882" alt='pic number 1 ' src="https://github.com/abboudcherine/kal281681/edit/main/README.md#members--cherine-abboud--kalkidan-mezgebe--ana-andrijasevic">

Data Preprocessing: We cleaned the dataset by removing unnecessary columns (e.g., 'ID') dealt with outliers . We also transformed the 'SMS Text' field using TF-IDF Vectorization to convert text data into a format suitable for machine learning.

Model Selection: We identified this as a binary classification problem, given the need to categorize SMS messages as either fraudulent or not. We experimented with several models, including Logistic Regression, Random Forest, and Support Vector Machines.
Hyperparameter Tuning: We used cross-validation to tune model parameters, adjusting settings like the number of trees in the Random Forest and the regularization strength in Logistic Regression.

Environment Setup: Our project was executed in a Jupyter notebook environment, with dependencies managed through Conda. The essential libraries included pandas, sklearn, numpy, matplotlib, and seaborn.

Section 3: Experimental Design

In our experiments, the primary objective was to determine the most effective machine learning model for accurately classifying SMS messages as fraudulent or legitimate. We established a baseline comparison using the accuracy of random guessing to assess the relative improvement offered by our models. For evaluation, we chose metrics such as accuracy, precision, recall, and the F1 score, which are crucial for understanding the balance between false positives and negatives in a binary classification context. These metrics were essential in ensuring that our model not only identified fraudulent messages accurately but also minimized the misclassification of legitimate messages. Through this experimental design, we were able to systematically compare the performance of different models and identify the most effective approach for SMS fraud detection.
