# Practical Application III: Comparing Classifiers
## Will a Customer Accept the Coupon?

Goto [prompt_III.ipynb](prompt_III.ipynb) for complete Jupyter Notebook.
------


### Overview:
The objective of this practical exercise is to evaluate and compare the effectiveness of several classifiers, including K Nearest Neighbor, Logistic Regression, Decision Trees, and Support Vector Machines, using a dataset that pertains to the marketing of banking products through telephone calls.


### Data:
The origin of the dataset is from the UCI Machine Learning repository [link](https://archive.ics.uci.edu/ml/datasets/bank+marketing), which contains information collected from various marketing campaigns conducted by a Portuguese banking institution.

------
### Results

#### Data insights:
1. previous, emp.var.rate, euribor3m, pdays, nr.employed are the columns having more than 0.23 imapct on the target column.
2. higher the duration and previous, higher the chances of subscribing to the term deposit and higher the emp.var.rate, euribor3m, pdays, nr.employed, lower the chances of subscribing to the term deposit.
3. admin is the most common job, followed by blue-collar and technician.
4. married people are more than single and divorced people.
5. most of the people have university degree.
6. most of the people have no credit in default.
7. most of the people have no housing loan.
8. most of the people have no personal loan.
9. most of the people are contacted through cellular.
10. most of the people are contacted in the month of may.
11. most of the people are contacted on the last day of the week.
12. most of the people are contacted for the first time.
13. there are more clinets who were not subscribed to the term deposit in the previous campaign.
- The data is imbalanced, which means the target column has more no values (only 11%) than yes values.
- The data is not normalized, which means the data is not in the same scale.

#### Modelling details:
- First data was verified and cleaned.
- few insights were drawn from the data.
- Baseline model was built using LogisticRegression.
- Comparision of DecisionTreeClassifier, KNeighborsClassifier, SVC, LogisticRegression was done.
- GridSearchCV was used to improve the model for all the classifiers.

#### Evaluation:
- All 4 classifiers were evaluated using accuracy score. Score was almost same for all the classifiers.
- LogisticRegression took the least time to train the model compared to other classifiers. It gave best scores even with GridSearchCV.
- SVC took the most time to train the model compared to other classifiers.
- For gridsearchcv, KNeighborsClassifier took the most time to train the model compared to other classifiers.
- precision, recall, f1-score, KNN gave the best results compared to other classifiers. with gridsearchcv, SVC was better.
