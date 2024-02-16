<div align="center">

# ******Diamonds Price Predictions****** </div> 

<div align="center">

	
 ![Captura de pantalla 2024-02-16 221627](https://github.com/AlanaCastillo/Ironhack-Project-Module-3/assets/141866356/ff64be2f-5aab-4715-a18a-6040b97f2995)</div> 







## 💎**Description**
Ironhack Madrid - Data Analytics Part Time - Sep 2023 - Project Module 3. 

This is a repository of the Machine Learning Competition on diamonds price prediction.
The objective of the project is to predict prices of diamonds based on different features by traing regression model.

The dataset used is in the following link:
https://www.kaggle.com/datasets/shivam2503/diamonds





## 💎**Dataset Description**
The dataset used in this contest contains different features about diamonds.

- **Id:** Identifier number
- **Price:** price of diamond
- **Cut:** is the shape and proportions of the diamond
- **Color:** is the hue of the diamond
- **Clarity:**  is the degree of purity of the diamond
- **City:** where the diamond was sold sold
- **Carat:** is the weight of the diamond
- **Depht:** is the distance from its top table to the culet at its base
- **Table:**  the facet which can be seen when the stone is viewed face up
- **x:** length 
- **y:** width 
- **z:** depth 



## 💎**Tecnologies**
-DBeaver

-Jupyter Notebook 

## 💎**Steps**


**Data Cleaning**   

- The dataset is stored with format .db I proceed to extract the data with DBeaver.
-  I use SQLite to be able toto get the tables.and export it to a CSV file


  **Data Preprocessing** 
  

- Categorical variables (cut, color, clarity and city) were encoded with LabenEncoder from scikit-learn.
- I concatenate features to make a single table.
- I sorted the columns so that they were in the same format as the test

**Features and Target** 
- Assigning the features as X (Features) and y (Target)
  
**Model Building** 
- Split the preprocessed dataset into training and testing sets using train_test_split from scikit-learn.
- Try 4 different models:
	1.	Linear Regression
	2.	RandomForest 💎
	3.	DecisionTree
	4.	GradientBoosting
- I decided to use the Random Forest Regressor model, which has been the one that has given me the best results.
- Obtain predictions of diamond prices, import to csv and upload to Kaggle competition.


## 💎 Project Structure

```bash
└── Ironhack-Project-Module-3 
    └── data
        ├── diamonds_train.csv
        ├── diamonds_test.csv
        ├── diamonds_train_enc.db
        ├── diamonds_test_enc.csv
        └── sample_submission.csv
    ├── models
        ├── Boost.ipynb
        ├── Desision Tree.ipynb
        ├── Linear.ipynb
        └── Random.ipynb

    ├── final submissions
        ├── model_1.csv
        └── model_2.csv
    ├── models
        ├── model_1.sav
        └── model_2.sav
    ├── .gitignore
    └── README.md
```






