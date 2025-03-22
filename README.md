# WIDS_Datathon_Uncovering_ADHD_In_Female_Brains
---

### **👥 Team Members**

| Vivian Song | @vsong1 | Performed data cleaning on quant datasets, built SVM models |
| Charu | @charuy2 | Performed data cleaning on categorical data, build rf and xgboost models |
| Christina Kaddouh | @ckaddouh | Built random forest classifier models, implemented boosting|
| Viswa | @vk1815918 | Implemented ensemble modeling for xgboost, random forrest, GBMs and cleaned datasets 


---

## **🎯 Project Highlights**

* Built a Random Forest Classifier using imputation, PCA, and scaling to predict both sex and ADHD likelihood from survey results alone
* Built SVM models using normalization, class balancing, and L1 regularization to more accurately predict based on both survey results and MRI scans
* Achieved an F1 score of 0.60861 and a ranking of 386 on the final Kaggle Leaderboard
* Printed out the decision tree to interpret model decisions
* Implemented KNN and iterative imputation, scaling, and removed missing values to optimize results within compute constraints

🔗 [WiDS Datathon 2025 | Kaggle Competition Page](https://www.kaggle.com/competitions/widsdatathon2025/overview)

---

## **👩🏽‍💻 Setup & Execution**

**Provide step-by-step instructions so someone else can run your code and reproduce your results. Depending on your setup, include:**

Load the datasets from the data folder onto your device: 
Open up the ____ script on google colab
Install the imports on the code
Specify the right dataset directories on google colab
Run the scripts 

---

## **🏗️ Project Overview**

**Describe:**
* We participated in this Kaggle competition as a part of the Break Through Tech AI program. The Kaggle competition is a part of the WiDS Datathon Global Challenge, which was developed with Ann S. Bowers Women’s Brain Health Initiative (WBHI) in collaboration with Cornell University and UC Santa Barbara. Datasets and support are provided by the Healthy Brain Network (HBN), the signature scientific initiative of the Child Mind Institute, and the Reproducible Brain Charts project (RBC). 

* The objective of the competition is to build a model to predict both an individual’s sex and their ADHD diagnosis using functional brain imaging data of children and adolescents and their socio-demographic, emotions, and parenting information.

* Neuropsychiatric disorders that occur in development, like anxiety, depression, autism, and attention deficit hyperactivity disorder, or ADHD, often differ in how and to what extent they affect males and females. ADHD occurs in about 11% of adolescents, with around 14% of boys and 8% of girls having a diagnosis. There is some evidence that girls with ADHD can often go undiagnosed, as they tend to have more inattentive symptoms which are harder to detect. Girls with ADHD who are undiagnosed will continue suffering with symptoms that burden their mental health and capacity to function. Our project will hopefully contribute to improving the accuracy of ADHD diagnoses in young girls.
---

## **📊 Data Exploration**

For this project we used the WiDS Datathon 2025 dataset that was provided by Kaggle.  The dataset also consisted of fMRI data, other socio-demographic features, and behavioral information including ADHD diagnosis and the sex of the participant (which we will predict). THe main datasets included:
The combined dataset of both quantitative and qualitative training data
THe fMRI data - represents brain connectivity patterns
The test dataset without solutions

Preprocessing: Primarily handled missing values using mode imputation as well as KNN imputation for both categorical and quantitative data. The numerical features are scaled as needed for certain models. All features within the data were already numerically encoded.

Challenges and Assumptions: The P2 column information was missing for a considerable number of columns which led to first adding a “no parent recorded” column” and then modified this to KNN imputation. 
Visualizations when Data Preprocessing:



---

## **🧠 Model Development**

* Models used: Mostly variations of decision tree models with boosting and PCA. Had some attempts with neural networks. In the end, applying ensemble methods to join these attempts together and boost accuracy. 
* Feature selection and Hyperparameter tuning strategies: employed one-hot encoding, PCA, and scaling. Used grid search for fine tuning neural network. 
* Training setup: 80/20 split of data for training/validation. Evaluated on F1 score, as well as how the model performed on Kaggle’s unique data in the competition. Baseline accuracy: 
---

## **📈 Results & Key Findings**

* Performance metrics: Kaggle Leaderboard score: , F1-score: 
* How your model performed overall: Ensemble methods increased robustness of the model overall. _____


---

## **🖼️ Impact Narrative**

**Answer the relevant questions below based on your competition:**

**WiDS challenge:**




1. What brain activity patterns are associated with ADHD; are they different between males and females, and, if so, how?
Based on the results of our correlation matrices, we see that hyperactivity and externalizing are the most closely correlated to outcomes of ADHD in both males and females. The primary difference in diagnosing ADHD between the sexes comes much farther down the line, in the fifth most correlated features. In females, internalizing is more significant, while in males, conduct problems are more relevant. 

2. How could your work help contribute to ADHD research and/or clinical care?
This work can help ADHD researchers know what to pay closer attention to when diagnosing ADHD in females vs. males. We see the characteristics/features that are most strongly correlated to a positive diagnosis, so these are things that doctors can pay closer attention to. 
---

## **🚀 Next Steps & Future Improvements**

**Address the following:**

* What are some of the limitations of your model?
* What would you do differently with more time/resources?
* What additional datasets or techniques would you explore?
** Not done yet, will fill in once we have our final model **
---
