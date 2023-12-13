# Bank Account Fraud Machine Learning Capstone 

### Overview and Business Understanding

Proactive detection of bank account application fraud is always a priority item for clients in the financial and banking industries. Detecting application fraud in a timely manner in hopes of preventing or reducing financial loss requires extensive time and effort. Advanced technology such as machine learning is not new, but increasing use cases and success allows for an expanded implementation scope. Machine learning models facilitate and expedite the detection process by identifying patterns of high risk account characteristics and features that are likely to be triggers of fraudulent activity. 

Clients who leverage machine learning models to detect fraudulent application patterns are more likely to reduce mean time to remediation by managing fraudulent event triggers before they are escalated to incidences. There is also increased chances of cost savings as less successful fraudulent applications equates to less financial loss and resources spent in remediation and subsequent payout. Practices such as these increase success rates and demonstrate consistent results, efficiency, and service confidence in clients' customers. Finally, resources and manpower previously dedicated to tedious fraud detection monitoring and management can be better utilized to expand the organization and provide oppportunity and time to dedicate to other focus areas. 

Our team at Deloitte seeks to create and implement a state-of-the-art machine learning model for the purpose of filling these gaps for clients in relevant industries. Our aim is to help our clients understand driving predictors of bank account application fraud and implement industry leading and effective detection processes. 

### Description of Data


**Data Source**: Bank Account Application Fraud: https://www.kaggle.com/datasets/sgpjesus/bank-account-fraud-dataset-neurips-2022/data

**EDA Techniques** 
Add EDA techniques used and why it was helpful to the data



### Data Understanding and Analysis



**Data Processing** 


**Modeling Techniques** 


**Success Metrics** 
add success metrics used and why 

When training our machine learning model for detecting bank account fraud, we employed a set of robust success metrics essential for evaluating its performance. Initially we utlized the ROC/AUC curve, offering a nuanced understanding of the model's ability to distinguish between fraudulent and legitimate transactions. This metric's effectiveness lies in its depiction of the trade-off between sensitivity (recall) and specificity, illustrating the model's performance across various thresholds. A high AUC score indicates a strong capability to classify between the two classes, serving as a reliable gauge of overall model performance.

Moreover, precision and recall were important success metrics in our evaluation strategy. Precision quantifies the accuracy of positive predictions made by the model, emphasizing the proportion of correctly identified fraudulent cases among all predicted positives. Recall, on the other hand, measures the model's capability to identify all actual positive cases, indicating the completeness of fraud detection. Therefore, recall proved more useful in our model evaluation. In our model we were looking for a high recall through changing the decision thresholds and different weights to the target classes. Through this and additional techiniques we were able to acheive a recall **0.63*. This coupled with our high AUC of 0.76 helped prove the effectiveness of our model. Additionally, balancing these two metrics ensures a comprehensive understanding of the model's effectiveness, guarding against false positives and false negatives, both critical in the context of bank account fraud detection. 

Finally, we created and analyzed confusion matrixes in order to see the models effectivness on a more granualar level. In turn this helped us improve out model throughout the process and identify areas of improvement for future tuning of our model. 

**Model Comparison** 


### Visualizations

1. Histogram
![CustomerAge](https://github.com/hacampbell1/capstoneproject/assets/140438534/7fb26f36-910a-489c-95eb-594c204d7ca4)

3. Heat Maps
4. Confusion Matrix

1. ROC Curve
2. AUC


### Description of Results and Performance 


### Conclusion and Next Steps 


### Works Cited 

1. Hillendahl, Alison. “Fraud Detection in Banking.” Experian Insights, Experian , 24 Aug. 2023, www.experian.com/blogs/insights/fraud-detection-in-banking/. 
2. “Banking Fraud Investigations - How Do Banks Detect Fraud?” Pindrop, Pindrop, 11 Sept. 2023, www.pindrop.com/blog/banking-fraud-detection. 
















