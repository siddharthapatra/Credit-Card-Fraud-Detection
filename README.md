# Credit Card Fraud Detection

## 1. Introduction
Fraudulent transactions have become a growing concern with the increase in digital payments worldwide. This project is focused on developing an effective and efficient credit card fraud detection model using machine learning techniques. It is an interesting task that reflects the real-world inclination of companies towards utilizing machine learning algorithms for identifying and preventing such fraudulent transactions.

## 2. Problem Statement
The aim of this project is to predict credit card frauds in a transactional dataset using various predictive models. In particular, the models would be trained to identify transactions that might be fraudulent so that customers are not charged for items they did not purchase.

## 3. Dataset
TThe dataset used contains transactions made by credit cards in September 2013 by European cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced; the positive class (frauds) account for 0.172% of all transactions. The dataset has been collected and analyzed during a research collaboration of Worldline and the Machine Learning Group (http://mlg.ulb.ac.be) of ULB (Universite Libre de Bruxelles) on big data mining and fraud detection. More details on current and past projects on related topics are available on http://mlg.ulb.ac.be/BuFence and http://mlg.ulb.ac.be/ARTML.

As the dataset was created using the PCA method, preprocessing of data has little scope. The imbalance between classes is compensated using oversampling and undersampling. The logistic regression, random forest, support vector machine, k-means are used within a cross-validation framework. Lastly, Recall and Accuracy are chosen as metrics while deducing the best classifier. A buffer section on outlier detection is added at the end.

## 4. Data Analysis and Preparation
#### 4.1 Exploratory Data Analysis (EDA)
An extensive EDA was carried out to understand the variables in the dataset and draw statistical conclusions. The distribution of variables was visualized, and significant variables playing crucial roles in segregating fraudulent and non-fraudulent transactions were identified. This analysis also helped to visualize the imbalance in data and the extent of it. Additionally, boxplots were used for visualizing outliers and evaluating the interquartile range of different features.

#### 4.2 Data Preparation
Due to the severe skewness of the dataset towards non-fraudulent transactions, undersampling or oversampling methods were considered for balance. Various techniques were discussed, and suitable methods were employed depending upon the specific requirements. Methods for scaling the variables and detecting outliers were also addressed.

## 5. Machine Learning Algorithms
Multiple machine learning algorithms were used in the project, including Random Forests, K-Nearest Neighbour, and Logistic Regression. Each algorithm was assessed using different statistical parameters like Precision, Recall, Accuracy, and others to determine its effectiveness in detecting fraudulent transactions.

#### 5.1 UnderSampling using Nearmiss Technique
For the undersampling of data, the Nearmiss technique was employed, which helped in balancing the data by reducing the instances of the majority class.

#### 5.2 OverSampling using SMOTE
The Synthetic Minority Over-sampling Technique (SMOTE) was used to over-sample the minority class (fraud transactions) by creating synthetic instances.

#### 5.3 Cross Validation
Cross-validation techniques were applied in the context of both undersampling and oversampling, ensuring that the models performed well on unseen data.

## 6. Model Training and Validation
Each machine learning model was trained and validated using a robust set of techniques:

A basic classification model was built using Random Forest.
Linear model: Logistic Regression was applied.
Ensemble technique: Random Forest was employed for improved results.
Non-linear algorithms: Support Vector Machine, Decision Tree and k-Nearest Neighbour were utilized.
The predictions on the test set were evaluated using validation metrics such as Precision, Recall, Accuracy, and Confusion Matrix. Additionally, ROC curves and Learning curves were drawn to assess the performance of the models.

## 7. Model Selection and Results Comparison
The models were compared based on their performance metrics, and the most suitable model was selected for this specific problem. This process highlighted the importance of choosing the correct metric for model selection in imbalanced datasets. In this case, Accuracy was not an appropriate metric due to the data imbalance, while Precision and Recall provided more valuable insights.

## 8. Visualization
Seaborn and matplotlib libraries were extensively used for visualizing the data distribution, performance of the models, and final results.

## 9. Conclusion and Future Work
This project provided a comprehensive understanding of handling imbalanced data and the application of different machine learning algorithms for credit card fraud detection. The project successfully demonstrated that machine learning can effectively detect fraudulent transactions by leveraging transaction details and customer information.

In future work, the performance of these models can be improved by incorporating more recent data and by trying out different preprocessing techniques and advanced machine learning and deep learning models.

## 10. FAQs
Q: Which are the best algorithms for credit card fraud detection?
A: Several algorithms can be used, including Random Forests, Logistic Regression, Support Vector Machines, K-Nearest Neighbour, Autoencoders, Isolation Forest, etc. The performance of these algorithms varies based on the dataset and needs to be evaluated using appropriate metrics.

Q: Why is Machine learning used in Credit Card Fraud Detection?
A: Machine learning algorithms can identify hidden patterns in the dataset and do not assume any predefined logic to differentiate between fraudulent and non-fraudulent transactions. Thus, they are well-suited to detect credit card frauds.
