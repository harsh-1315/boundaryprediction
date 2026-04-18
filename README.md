&#x20;IPL Boundary Prediction using Random Forest



&#x20;Overview



Cricket is a highly dynamic sport where every ball can influence the outcome of a match. In tournaments like the Indian Premier League (IPL), boundary events such as fours and sixes play a crucial role in determining match momentum.



This project focuses on predicting boundary outcomes using machine learning techniques. A Random Forest classifier is applied on ball-by-ball IPL data to classify deliveries into:



\* No Boundary

\* Four

\* Six





&#x20;Dataset



The dataset used in this project is the IPL ball-by-ball dataset.



&#x20;Files Included:



\* `deliveries.csv`





Dataset Details:



\* Total Records: \*\*179,078\*\*

\* Total Features: \*\*21\*\*

\* Target Variable: `boundary\_class`







&#x20;Features Used



The following features were used to train the model:



\* `over` – Represents match progression

\* `ball` – Ball number within an over

\* `over\_ball` – Combined feature (over + ball/10)

\* `is\_powerplay` – Indicates powerplay phase (overs 1–6)

\* `is\_death` – Indicates death overs (overs 16–20)

\* `pressure\_index` – Interaction feature (over × ball)



&#x20;Model Used



\* \*\*Random Forest Classifier\*\*



&#x20;Why Random Forest?



\* Handles non-linear relationships effectively

\* Reduces overfitting using ensemble learning

\* Works well with structured datasets





&#x20;Technologies Used



\* Python

\* Pandas \& NumPy

\* Matplotlib

\* Scikit-learn







&#x20;Model Performance



| Metric    | Value  |

| --------- | ------ |

| Accuracy  | 0.8405 |

| Precision | 0.7064 |

| Recall    | 0.8405 |

| F1 Score  | 0.7676 |







&#x20;Observations



\* The model performs very well for \*\*non-boundary deliveries\*\*

\* Performance is weaker for \*\*fours and sixes\*\*

\* This is mainly due to \*\*class imbalance\*\* in the dataset







Visualizations



The following graphs are included in the project:



\* Feature Correlation Heatmap

\* Confusion Matrix

\* Feature Importance Plot

\* ROC Curve

\* Learning Curve

\* Boundary Class Distribution





&#x20;Project Structure



IPL-Boundary-Prediction/

│── data/

│   ├── deliveries.csv

│   ├── matches.csv

│── IPL\_Boundary\_Prediction\_RandomForest.ipynb

│── heatmap.png

│── confusion\_matrix.png

│── feature\_importance.png

│── learning\_curve.png

│── roc\_curve.png

│── README.md







&#x20;How to Run



1\. Clone the repository

2\. Install required libraries

3\. Open the notebook

4\. Run all cells







&#x20;Conclusion



This project demonstrates how machine learning can be applied to sports analytics. The Random Forest model successfully captures patterns in match data and provides meaningful predictions based on match context.







&#x20;Future Improvements



\* Handle class imbalance using SMOTE or resampling

\* Add more contextual features (player data, venue, etc.)

\* Try advanced models like XGBoost or Neural Networks





&#x20;Authors



\* Harsh Dodia

\* Muskan Padhiar

\* Nishita Sheth

\* Ankur Singh



