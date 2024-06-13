In this project, I undertook a comprehensive analysis of customer churn, focusing on identifying trends and building predictive models to forecast churn. The project began with importing a suite of essential libraries, including pandas, numpy, seaborn, matplotlib, plotly, scikit-learn, and xgboost. These libraries provided the necessary tools for data manipulation, visualization, and model building.

The dataset was sourced from a CSV file and loaded into a pandas DataFrame. Initial data cleaning steps involved dropping irrelevant columns such as 'Surname', 'Gender', 'RowNumber', and 'CustomerId' to streamline the dataset and focus on the most impactful features. Label encoding was applied to the 'Geography' column to convert categorical data into numerical form, which is a requirement for many machine learning algorithms. The label encoding mapped 'France', 'Germany', and 'Spain' to 0, 1, and 2, respectively.

To explore the data, I created visualizations using Seaborn and Plotly. Seaborn's displot function was employed to generate distribution plots of features like Age, Estimated Salary, and Credit Score, segmented by geography and churn status. This helped in understanding the distribution and density of these features across different groups. Plotly was used to create interactive donut charts, illustrating the distribution of churners and non-churners by geography, and overall customer distribution. These visualizations provided intuitive insights into how different features and geographic locations impact customer churn.

For the predictive modeling, I implemented two machine learning classifiers: XGBoost and Random Forest. The dataset was split into training and test sets using an 80-20 split ratio. Feature scaling was performed using StandardScaler to standardize the features, ensuring that they have a mean of zero and a standard deviation of one. This step is crucial for algorithms that are sensitive to the scale of input data.

The XGBoost classifier was initialized with specific parameters to optimize its performance. After training the model on the training data, predictions were made on the test set. The model's performance was evaluated using metrics such as accuracy, F1 score, confusion matrix, and a classification report. The XGBoost model achieved an accuracy of 85.6% and an F1 score of 0.57, indicating its capability to handle the churn prediction task, though with some limitations in balancing precision and recall for the minority class (churners).

Next, I trained a Random Forest classifier, which typically performs well on structured data. Similar to XGBoost, the model was trained on the training set, and predictions were made on the test set. The Random Forest classifier achieved an accuracy of 87.05% and an F1 score of 0.59, outperforming the XGBoost model. The confusion matrix and classification report indicated better precision and recall balance, making Random Forest a more reliable choice for this specific task.


To summarize, this project successfully demonstrated the application of data cleaning, visualization, and machine learning techniques to predict customer churn. The Random Forest classifier emerged as the superior model, providing valuable insights and actionable predictions for managing customer retention strategies. This analysis underscores the importance of leveraging data-driven approaches to understand and mitigate customer churn.




