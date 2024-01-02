# kal281681                                         AI machine learning project 

### dataset : SafeComm Digital Security Solutions
### members : 
- cherine Abboud ,289351
- kalkidan Mezgebe ,281681
- Ana Andrijasevic ,285991

# Section 1: Introduction

In this project, we developed a machine learning model for SafeComm Digital Security Solutions to identify fraudulent SMS messages. The prevalence of SMS-based fraud poses significant risks, and our model aims to mitigate these by automatically flagging suspicious messages. We utilized an anonymized dataset provided by a telecom partner, containing a mix of regular and potentially fraudulent SMS messages.

# Section 2: Methods

Our approach involved several key steps:
Eda and visulisaton : we conducted a  thorough exploratory data analysis (EDA) to gain insights into the dataset. This includes:
Checking for missing values.
Analyzing the distribution of fraudulent vs. non-fraudulent SMS.
Understanding the nature and variety of SMS texts.
Exploring any patterns or trends over time (based on the 'Date and Time' column).



Data Preprocessing: We cleaned the dataset by removing unnecessary columns (e.g., 'ID') dealt with outliers . We also transformed the 'SMS Text' field using TF-IDF Vectorization to convert text data into a format suitable for machine learning.

Model Selection: We identified this as a binary classification problem, given the need to categorize SMS messages as either fraudulent or not. We experimented with several models, including Logistic Regression, Random Forest, and Support Vector Machines.
Hyperparameter Tuning: We used cross-validation to tune model parameters, adjusting settings like the number of trees in the Random Forest and the regularization strength in Logistic Regression.

Environment Setup: Our project was executed in a Jupyter notebook environment, with dependencies managed through Conda. The essential libraries included pandas, sklearn, numpy, matplotlib, and seaborn.

# Section 3: Experimental Design

In our experiments, the primary objective was to determine the most effective machine learning model for accurately classifying SMS messages as fraudulent or legitimate. We established a baseline comparison using the accuracy of random guessing to assess the relative improvement offered by our models. For evaluation, we chose metrics such as accuracy, precision, recall, and the F1 score, which are crucial for understanding the balance between false positives and negatives in a binary classification context. These metrics were essential in ensuring that our model not only identified fraudulent messages accurately but also minimized the misclassification of legitimate messages. Through this experimental design, we were able to systematically compare the performance of different models and identify the most effective approach for SMS fraud detection.

# section 4: results 

Our analysis led to several important findings:

Model Performance: Logistic Regression emerged as the top-performing model, balancing accuracy, precision, recall, and F1 score effectively.
Key Indicators: The model identified specific keywords as significant indicators of fraudulent messages, providing valuable insights for future fraud detection strategies.
Model Comparison: While Logistic Regression was the best fit for our needs, other models like Random Forest and SVM also showed good performance but were less efficient for real-time analysis.
Misclassifications Analysis: The model occasionally misclassified urgent-sounding legitimate messages as fraudulent, suggesting an area for improvement.
Efficiency and Scalability: Logistic Regression proved to be both efficient and scalable, making it suitable for processing large datasets.
These results highlight the effectiveness of Logistic Regression in SMS fraud detection and point towards areas for future enhancement.

# Section 5: Conclusions
Our project successfully demonstrated the capability of machine learning techniques in detecting fraudulent SMS messages, providing a valuable asset to SafeComm's digital security toolkit. The most significant outcome of this project was the selection of Logistic Regression as our optimal model. This choice was informed by its balance of performance, interpretability, and efficiency in classifying SMS messages. Although the model shows promising results in fraud detection, there remain areas for future exploration. These include the incorporation of more sophisticated natural language processing techniques and the adaptation of the model for real-time detection systems. The limitations of the current approach and the continuously evolving nature of SMS-based fraud present ongoing challenges and opportunities for further research and development in this field.

3 / 3
