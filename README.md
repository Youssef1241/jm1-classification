## 🧠 Machine Learning Analysis and Classification  
_by Youssef Tarek_

---

Full analysis and classification of the  
[Jm1 dataset](https://www.openml.org/search?type=data&sort=runs&id=1053&status=active) by Halstead and McCabe.

The dataset is used to predict whether a module or function in a software program will contain a defect based on several features, including but not limited to: lines of code, design complexity, percentage of difficulty, and program length. These input features and the way they are obtained were introduced by researchers McCabe and Halstead to evaluate software programs.

---

## 📊 Dataset Description

The features represent different aspects of a software program. There are:
- **5 features** related to the length of the program  
- **3 features** calculated using McCabe’s metrics  
- **12 Halstead features** (4 base features and 8 derived features)

**Label:**  
`defects: {False, True}` — indicates whether a module has one or more reported defects.

---

## 📈 Label Distribution

<img width="415" height="409" alt="image" src="https://github.com/user-attachments/assets/8823d6de-537f-40e6-82a4-b015f1b5ce59" />



A main problem with this dataset is its unbalanced distribution, the project attempts to handle this with methods like oversampling, changing class weights, and changing probability thresholds.

---

## 🏋️‍♂️ Model Training

Three models were used to optimize this dataset: Random Forest Classifier, Logistic Regression, and K-Nearest Neighbor.

## 🤖 Model Evaluation

We evaluated three models using multiple metrics, including ROC-AUC, F1 score, and recall.

<img width="567" height="455" alt="image" src="https://github.com/user-attachments/assets/53596fa4-bed0-423d-a093-b89be7848842" />

Overall ranking of models:
- **Random Forest:** lowest performance  
- **Logistic Regression:** medium performance  
- **K-Nearest Neighbors:** best performance


