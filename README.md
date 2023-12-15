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


When training our machine learning model for detecting bank account fraud, we employed a set of robust success metrics essential for evaluating its performance. Initially we utlized the ROC/AUC curve, offering a nuanced understanding of the model's ability to distinguish between fraudulent and legitimate transactions. This metric's effectiveness lies in its depiction of the trade-off between sensitivity (recall) and specificity, illustrating the model's performance across various thresholds. A high AUC score indicates a strong capability to classify between the two classes, serving as a reliable gauge of overall model performance.

Moreover, precision and recall were important success metrics in our evaluation strategy. Precision quantifies the accuracy of positive predictions made by the model, emphasizing the proportion of correctly identified fraudulent cases among all predicted positives. Recall, on the other hand, measures the model's capability to identify all actual positive cases, indicating the completeness of fraud detection. Therefore, recall proved more useful in our model evaluation. In our model we were looking for a high recall through changing the decision thresholds and different weights to the target classes. Through this and additional techiniques we were able to acheive a recall **0.63*. This coupled with our high AUC of 0.76 helped prove the effectiveness of our model. Additionally, balancing these two metrics ensures a comprehensive understanding of the model's effectiveness, guarding against false positives and false negatives, both critical in the context of bank account fraud detection. 

Finally, we created and analyzed confusion matrixes in order to see the models effectivness on a more granualar level. In turn this helped us improve out model throughout the process and identify areas of improvement for future tuning of our model. 


### Visualizations

1. Histogram
<img width="400" src = "https://github.com/hacampbell1/capstoneproject/assets/140438534/7fb26f36-910a-489c-95eb-594c204d7ca4">
<img width="400" src = "https://github.com/hacampbell1/capstoneproject/assets/140438534/e83bd679-bcda-4a49-ac04-30b86814a9b1"
<img width="400" alt="Capture3" src="https://github.com/hacampbell1/capstoneproject/assets/140438534/c4ffdd27-b79e-4e87-84d9-7593abe25b0e">
<img width="400" alt="Capture4" src="https://github.com/hacampbell1/capstoneproject/assets/140438534/8336ae69-bed3-4427-aaf8-b48a5a4a884c">


3. Feature Importance: Undersampling
<img width="400" alt="Capture" src="https://github.com/hacampbell1/capstoneproject/assets/140438534/2b3b0dd0-2711-4278-a724-384822cee8d8">
<img width="400" alt="Capture1" src="https://github.com/hacampbell1/capstoneproject/assets/140438534/7766119b-6f85-4825-8655-110716083adc">

4. Feature Importance: Oversampling
<img width="400" alt="Capture6" src="https://github.com/hacampbell1/capstoneproject/assets/140438534/3784bf50-85f4-4ab7-9751-8fa379ee1a80">
<img width="400" alt="Capture5" src="https://github.com/hacampbell1/capstoneproject/assets/140438534/30b8b121-38ee-4f06-99bb-4d44194960de">

6. Heat Maps
<img width="400" src = "https://github.com/hacampbell1/capstoneproject/assets/140438534/323910c5-633f-4c17-8a11-6213dedce471">

7. Confusion Matrix
<img width="400" src = "https://github.com/hacampbell1/capstoneproject/assets/140438534/5801422f-7c73-4414-bed3-4e108cff8545">

1. ROC Curve


3. AUC


### Description of Results and Performance 


### Conclusion and Next Steps 

The most successful machine learning models are those in which consistent adjustments are made to best suite the business needs and improve model outcomes. Our team suggests the following next steps for continued improvement and positive impact. We first propose the client performs focused research into the most impactful fraud factors identified by our model. 

Although slight within the same industry, these predictors could vary from client to client. Leveraging these predictors as they best correlate to the client’s known fraudulent patterns and trends is recommended. As this directed research is being performed, it’s likely model scope or business need in relation to model output will be adjusted. Utilizing domain knowledge and investigating the most impactful fraud predictors are encouraged. In a similar fashion, continued development of the fraud account application machine learning model via the use of additional black box models such as Neural Networks is recommended. This will improve performance in large-scale data, improve efficiency and adaptaiblity. 

Finally, we suggest exploring additional model performance metrics that accurately reflect the performance of the model. In addition to the ROC AUC curve, Confusion Metrics, and classification tasks such as precision and recall other opportunities for exploration include regression tasks such as mean squared error (MSE), mean absolute error (MAE) and R-squared. Taking these recommendations into consideration will enhance overall model performance and provide a wide range of visibility into the most impact bank account fraud application factors and set our clients up for continued success.  




### Works Cited 

1. Hillendahl, Alison. “Fraud Detection in Banking.” Experian Insights, Experian , 24 Aug. 2023, www.experian.com/blogs/insights/fraud-detection-in-banking/. 
2. “Banking Fraud Investigations - How Do Banks Detect Fraud?” Pindrop, Pindrop, 11 Sept. 2023, www.pindrop.com/blog/banking-fraud-detection. 
















