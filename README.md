# House-Prediction-Model

## Introduction

The repository here, is a ML prediction model based off of a Chennai Dataset on Kaggle , for various locations in Chennai. These will be the catalyst for us to predict the price of any property based off of a few set
features ( discussed later ) which will yield a predicted price result.  

## Dataset 📊

**File name** : Housing-Prices-in-Chennai.csv  
**Number of Rows** : 5014  
**Target Variables for this Project** : Price in INR  
**Key Features implemented** :   

"Area", "Location", "No. of Bedrooms", "Resale", "Hospital", "LiftAvailable", "School", "CarParking",
    "Gymnasium", "SwimmingPool", "PowerBackup", "ClubHouse", "ShoppingMall", "VaastuCompliant",
    "Children'splayarea", "GolfCourse", "AC", "AreaPerBedroom", "IsLuxury"  

*Additionally , the following features have also be implemented to achieve a higher score of accuracy : AreaPerBedroom [ Area / No. of Bedrooms ] , IsLuxury [ SwimmingPool + Gym + AC + PowerBackup > 2 ]*

## Model Information 🔎

**Algorithm Implemented** : Gradient Boosting Regressor  
**Feature Engineering** : IsLuxury , AreaPerBedroom [ as mentioned above ]  
**Target** : Log1p(Price) [ for better computing results , and to reduce skewness ]  

## Performance Report 🦾  

We implement the conventional 80-20 training split and get the following results :   

R^2 Score : ~0.32  
MAE : 12.3 Lakh INR  
RMSE : 18.9 Lakh INR  

![image](https://github.com/user-attachments/assets/3bfcf3e0-2614-4800-8cfc-fe9a228de311)

## How to Run and Install 🔽  

### Dependencies  
pandas
numpy
scikit-learn

### Install By  

pip install pandas numpy scikit-learn
