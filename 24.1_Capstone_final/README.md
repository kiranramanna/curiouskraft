### User Utterence Intent identification and Classification

This project will develop a model that takes as input a natural language question of the user query and provides an intent classification of the user query. If the user query belongs to the scope of the model (user intents defined in the Clinc-150 dataset), the output

**Author**
@kiranramanna

#### Executive summary
The project aims to classify the intent of user queries using the Clinc-150 dataset, with a focus on identifying out-of-scope queries. The purpose of this project is to provide an effective and accurate way to classify user intents, which is essential for developing conversational AI systems that can understand and respond to natural language queries.

#### Rationale
The ability to accurately classify user intents is crucial for developing conversational AI systems that can effectively respond to user queries. Understanding the user's intent allows the system to provide relevant and accurate responses, leading to a better user experience. Moreover, identifying out-of-scope queries is equally important as it enables the system to recognize when it is unable to fulfill the user's request and provide a suitable response.


#### Research Question
The primary research question is how to classify user intents accurately and efficiently, with a particular focus on identifying out-of-scope queries.


#### Data Sources
The Clinc-150 dataset will be used for this project, which consists of 150 distinct intents and over 10,000 unique queries. The dataset also includes out-of-scope queries that do not fall into any of the predefined intents, which makes it ideal for this project.

#### Methodology
The project will use classification models as listed below:
- DecisionTreeClassifier,
- LogisticRegression,
- KNeighborsClassifier,
- SVC,
- RandomForestClassifier,
- XGBClassifier


#### Results
What did your research find?
The project aims to develop an accurate and efficient intent classification model that can correctly identify user intents and out-of-scope queries. The results will be measured using standard classification metrics, such as accuracy, precision, recall, and F1-score. The model's performance will be compared with existing state-of-the-art models, and the results will be analyzed to determine the model's effectiveness.

#### Next steps
The next steps would be to deploy the intent classification model in a conversational AI system and evaluate its performance in a real-world scenario. The model could be further improved by fine-tuning hyperparameters or using more advanced deep learning techniques. Additionally, the out-of-scope queries could be further analyzed to determine common patterns or themes, which could aid in improving the model's performance.

#### Outline of project

- [Link to notebook 1](final_capstone.ipynb)

##### Contact and Further Information
If you have any further questions or need additional assistance, please feel free to ask.