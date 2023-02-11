# Phase-3-project
## Classification of water wells in Tanzania
![waterwell](https://user-images.githubusercontent.com/117116395/218067424-85605530-08c5-4050-9635-a50682da47a1.jpg)
## Introduction
Access to clean water is a fundamental human need and a major challenge for many developing countries, including Tanzania. With a population of over 57 million, providing clean water to all citizens is a critical task. There are many water points already established in Tanzania, but some are in dire need of repair while others have completely failed.
<br />
<br />
In order to address this challenge, we aim to build a classifier to predict the condition of water wells based on information such as the type of pump used and the installation date. This tool will be instrumental in helping NGOs locate wells that need repair and the government of Tanzania to identify patterns in non-functional wells, which can inform the construction of new wells. This is a ternary classification problem, but can be designed to be binary. With this project, we hope to improve access to clean water for the people of Tanzania and help address this critical need.

## Business Understanding
Tanzania struggles to provide clean water to its population due to the failure or in need of repair of some of its existing water wells.There is a need to improve access to clean water in Tanzania. With a population of over 57 million, it is important to ensure that as many water wells as possible are functional and providing clean water to those who need it. 
<br />
The lack of access to clean water not only affects the health and well-being of the population, but also hinders the economic and social development of the country.. By building a classifier that can predict the condition of a water well, organizations such as NGOs and the government can more efficiently identify and repair non-functional wells and make informed decisions about the construction of new wells.The benefits of this project include improved water accessibility for the population of Tanzania, better management of existing wells, and data-driven decision-making for the government.
<br>
## Main Objectives
To build a classifier that can predict the condition of water wells based on information about the class the waterpoints belong to: functional, functional but need some repairs, and non-functional.

## Specific Objectives
Conducting a thorough exploratory data analysis of the dataset to understand the relationships between each feature and the labels.
To develop a classifier that accurately predicts the condition of water wells, using the collected data.
To evaluate the performance of the classifier and make improvements as necessary.
To measure the impact of the classifier on the access to clean water in Tanzania, and to make improvements as necessary to ensure ongoing success.


## Data Preparation and modeling.
Assessing the Data: The dataset had almost 60,000 instances with 39 features, mostly of nominal categorical type. It was a multiclass classification problem with three potential classes for each instance.
<br>
Data Cleaning: The dataset had a notable number of missing values, which were filled in using the mean, median, or mode based on the situation.
<br>
Exploring the Data/Selecting Features: During the cleaning process, data  was examined and concurrent familiarization with the values was done. The relevant features were then selected. The features were categorized into Useless to the model, Missing Too Much Data, Redundant, Potentially Relevant, and Potentially Relevant but with high cardinality. After choosing the Potentially Relevant features, I further investigated their correlation to the classes.
<br>
*Making Predictions:* A baseline model was selected and various classifiers for modeling and the most promising ones fine-tuned. Recall and Accuracy were used as evaluation metrics. By utilizing a Random Forest Classifier, a 72% accuracy score was obtained and recall values of 0.75, 0.60, and 0.72 for the 'functional', 'functional needs repairs', and 'non-functional' categories. The 'functional needs repairs' category was the minority class, with a recall of 0.60.


## Conclusion.

* By utilizing a Random Forest Classifier, I obtained a 72% accuracy score and recall values of 0.75, 0.60, and 0.72 for the three categories, 'functional', 'functional needs repairs', and 'non-functional'. The minority class was the category with a recall of 0.60.
* The Ministry of Water could benefit significantly from this capability to predict water point statuses since it would enable them to prioritize site visits.

## Recommendations

* I recommend the Ministry of Water utilize the predictive model to develop a strategy for prioritizing waterpoint site visits. The model recommends that waterpoints predicted to be 'functional needs repairs' and 'non functional' be given priority status, while waterpoints predicted to be 'functional' be inspected on a routine basis and to check for any misclassified waterpoints.

* By creating a more effective maintenance program, the Ministry can reduce costs and allocate those savings towards expanding the water infrastructure. Additionally, the accuracy of the model and the Ministry's improved maintenance program can be used to showcase the government's progress and attract international aid.


