# Predicting-the-knowledge-level-of-Users
## Table of Contents  
1. [Abstract](#abstract)  
2. [Introduction](#introduction)  
3. [Methodology](#methodology)  
4. [Results](#results)  
5. [Discussion](#discussion)  
6. [Conclusion](#conclusion)  
7. [References](#references)  

---

## Abstract  
The primary goal of this project is to predict/classify a user's knowledge level based on variables such as study time, revision frequency, and exam performance. The dataset from undergraduate students at Gazi University (2009 semester) on Electrical DC Machines was analyzed using KNN and Decision Tree classifiers. Key findings include:  
- Decision Tree classifiers outperformed KNN in accuracy (~92% vs. ~85%) and interpretability.  
- Study time, revision frequency, and exam performance were critical predictors.  
- Recommendations include incorporating additional factors like keystrokes or mouse movements for future studies.
  
## Introduction  
Accurately identifying users’ knowledge levels is crucial for improving personalised online 
learning experiences in learning management systems. Learning systems and personalised 
teaching methods can be improved by having a better understanding of users’ knowledge 
levels. Educational institutions and platforms can adjust their teaching strategies, content 
distribution, and interventions to suit the unique needs of individual students by accurately 
identifying users’ knowledge levels. This may result in enhanced learning opportunities, 
better student engagement, and more successful educational outcomes. 
 To appropriately determine each user's knowledge level, it is essential to consider pertinent 
attributes and the relationship between them to properly grasp a student's or user's expertise 
on a certain subject. In addition, the model used to predict the knowledge level of each user 
based on the provided attributes is crucial. This report uses the user knowledge modelling 
dataset to study the relationships between the dataset's attributes and predict the user's 
knowledge level using KNN and a decision tree classifier. The main contributions of this 
paper are: 
• Understanding and assessing the relationship between each attribute and reporting on 
their significance to our goal. 
• Predicting the knowledge level of a user given the value for each attribute 
• Recommendations for improving the accuracy of predicting the knowledge level of 
users. 

## Methodology
### Dataset
The user knowledge modelling dataset is an actual dataset of undergraduate students’ 
knowledge status regarding the subject of Electrical DC Machines that was acquired from the 
Department of Electrical Education at Gazi University in the 2009 semester. It consists of a 
total of 403 instances and 6 attributes(including the target value). The 6 attributes are UNS 
(The knowledge level of the user), STG (The degree of study time for goal object materials), 
SCG (The degree of repetition number of users for goal object materials), STR (The degree 
of study time for related objects with goal object), LPR (The exam performance of user for 
related objects with goal object), PEG (The exam performance of user for goal objects), and 
PEG (The exam performance of user for related objects with goal objects). 

The dataset was already divided into training and testing sets, with 145 records in the testing 
set. The xls files were converted to csv files and were loaded and viewed using the pandas 
library. To clean the data, the following steps were taken: changing the data type, checking 
for outliers, checking for duplicates and typos, and checking for impossible values and 
missing values. Before preprocessing, the train and test data were combined. The heads of the 
columns contained white space. Additionally, there was a data entry error in the UNS 
column, which was fixed. Other than that, the STG contained a few outliers, but additional 
examination of the numbers revealed that they appeared to be significant to the study. As a 
result, it wasn't removed. The dataset does not contain any duplicates, errors, impossible, or 
missing values. Finally, each attribute's datatype was updated.

