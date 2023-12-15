# Bank Account Fraud Machine Learning Capstone 

### Overview and Business Understanding

Proactive detection of bank account application fraud is always a priority item for clients in the financial and banking industries. Detecting application fraud in a timely manner in hopes of preventing or reducing financial loss requires extensive time and effort. Advanced technology such as machine learning is not new, but increasing use cases and success allows for an expanded implementation scope. Machine learning models facilitate and expedite the detection process by identifying patterns of high risk account characteristics and features that are likely to be triggers of fraudulent activity. 

Clients who leverage machine learning models to detect fraudulent application patterns are more likely to reduce mean time to remediation by managing fraudulent event triggers before they are escalated to incidences. There is also increased chances of cost savings as less successful fraudulent applications equates to less financial loss and resources spent in remediation and subsequent payout. Practices such as these increase success rates and demonstrate consistent results, efficiency, and service confidence in clients' customers. Finally, resources and manpower previously dedicated to tedious fraud detection monitoring and management can be better utilized to expand the organization and provide oppportunity and time to dedicate to other focus areas. 

Our team at Deloitte seeks to create and implement a state-of-the-art machine learning model for the purpose of filling these gaps for clients in relevant industries. Our aim is to help our clients understand driving predictors of bank account application fraud and implement industry leading and effective detection processes. 

### Description of Data


**Data Source**: Bank Account Application Fraud: https://www.kaggle.com/datasets/sgpjesus/bank-account-fraud-dataset-neurips-2022/data

**EDA Techniques** 
We started going through our dataset primarily with .info() to understnad each variable we were dealing with, as well as the possible values. We had 25 categorical and 5 variables that could be one of a set number of values. To better understand what these values could be, we had to go and search the dataset and associated documents which listed what each value represented and what they could possibly be. Upon disocvering this, we were able to understand each vaiable as whether it related to the technology used for the applicaation, background information about the applicant themselves, or information on the application itself.

After understanding what each variable was and how it was associated or could ahve confounding impact with other variables, we went and searched basic summary statistics (mean, median, mode, etc.) or each variable to understand the range we were working with (eventuallyy we would standardize for better analysis). Next, we created various plots, often bar charts, to look at the distribution of variables as well as any outliars that could give us more insight into later analysis or each variable and how it could affect the likelihood of fraud. 

Next, as out target was understanding the relationship between each variable and it's association with fraud, we created a heatmap to look for any associations between all variables. We predominantly were focusing on relationships with variables and the target variable, fraud_value, and we did see a range of correlation leading to a starting point for us to analyze and develop our model.


### Data Understanding and Analysis


When training our machine learning model for detecting bank account fraud, we employed a set of robust success metrics essential for evaluating its performance. Initially we utlized the ROC/AUC curve, which offered an understanding of the model's ability to distinguish between fraudulent and legitimate transactions. This success metric allows us to see the trade-off between sensitivity and specificity of fruaduluent and non-fraudulent accounts. A high AUC score indicates a strong capability to classify between the two classes, serving as a reliable gauge of overall model performance.

Moreover, precision and recall were important success metrics in our evaluation strategy. Precision quantifies the accuracy of positive predictions made by the model, emphasizing the proportion of correctly identified fraudulent cases among all predicted positives. Recall, on the other hand, measures the model's capability to identify all actual positive cases, indicating the completeness of fraud detection. Therefore, recall proved more useful in our model evaluation. In our model we were looking for a high recall through changing the decision thresholds and different weights to the target classes. Through this and additional techiniques we were able to acheive a recall **0.63*. This coupled with our high AUC of 0.76 helped prove the effectiveness of our model. Additionally, balancing these two metrics ensures a comprehensive understanding of the model's effectiveness, guarding against false positives and false negatives, both critical in the context of bank account fraud detection. 

Finally, we created and analyzed confusion matrixes in order to see the models effectivness on a more granualar level. In turn this helped us improve out model throughout the process and identify areas of improvement for future tuning of our model. 


### Visualizations

1. Histogram
![download](https://github.com/hacampbell1/capstoneproject/assets/140438534/597606a7-becd-4c3f-a2a3-a6f84eeedde7)
![download (5)](https://github.com/hacampbell1/capstoneproject/assets/140438534/d2a76b79-5c79-4252-922d-a657d248343c)


3. Feature Importance: Undersampling
![download (6)](https://github.com/hacampbell1/capstoneproject/assets/140438534/7aff70a6-b7b4-42c7-b460-9bb7fa10fab7)

![download (7)](https://github.com/hacampbell1/capstoneproject/assets/140438534/9717b0eb-20ac-42c0-8484-0e1004328c3f)

4. Feature Importance: Oversampling
![download (3)](https://github.com/hacampbell1/capstoneproject/assets/140438534/f808f4fd-b839-447e-a2bd-e08d594918b0)
![download (4)](https://github.com/hacampbell1/capstoneproject/assets/140438534/f169df55-91a6-48dc-9b4f-5e9c4e9291e9)

5. SMOTE's Impact on Class Distribution
 ![download (4)](https://github.com/hacampbell1/capstoneproject/assets/140438534/a53e3f8f-cdeb-41d5-a964-6b4cf18864cf)
   
7. Heat Maps
![download](https://github.com/hacampbell1/capstoneproject/assets/140438534/cc25b0b9-c65a-48ea-b0c5-f2574074c986)


8. Confusion Matrix
![download (2)](https://github.com/hacampbell1/capstoneproject/assets/140438534/c3475555-1dba-45a5-93c9-386d18417ae5)
![download (1)](https://github.com/hacampbell1/capstoneproject/assets/140438534/925b3855-a6c4-47b2-8f92-ffcf8a0de6d1)

9. ROC Curve


10. AUC


### Description of Results and Performance 


### Conclusion and Next Steps 

The most successful machine learning models are those in which consistent adjustments are made to best suite the business needs and improve model outcomes. Our team suggests the following next steps for continued improvement and positive impact. We first propose the client performs focused research into the most impactful fraud factors identified by our model. 

Although slight within the same industry, these predictors could vary from client to client. Leveraging these predictors as they best correlate to the client’s known fraudulent patterns and trends is recommended. As this directed research is being performed, it’s likely model scope or business need in relation to model output will be adjusted. Utilizing domain knowledge and investigating the most impactful fraud predictors are encouraged. In a similar fashion, continued development of the fraud account application machine learning model via the use of additional black box models such as Neural Networks is recommended. This will improve performance in large-scale data, improve efficiency and adaptaiblity. 

Finally, we suggest exploring additional model performance metrics that accurately reflect the performance of the model. In addition to the ROC AUC curve, Confusion Metrics, and classification tasks such as precision and recall other opportunities for exploration include regression tasks such as mean squared error (MSE), mean absolute error (MAE) and R-squared. Taking these recommendations into consideration will enhance overall model performance and provide a wide range of visibility into the most impact bank account fraud application factors and set our clients up for continued success.  




### Works Cited 

1. Hillendahl, Alison. “Fraud Detection in Banking.” Experian Insights, Experian , 24 Aug. 2023, www.experian.com/blogs/insights/fraud-detection-in-banking/. 
2. “Banking Fraud Investigations - How Do Banks Detect Fraud?” Pindrop, Pindrop, 11 Sept. 2023, www.pindrop.com/blog/banking-fraud-detection. 
















