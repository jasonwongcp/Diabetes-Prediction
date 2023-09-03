# 🚀 Project Problem Statement 📋

The rising prevalence of diabetes is posing significant challenges to healthcare systems in the U.S., leading to substantial healthcare expenditures. To address this issue and mitigate the burden on healthcare costs, the project aims to develop and deploy machine learning models that can accurately predict the risk of developing diabetes based on readily available health datasets. The objective is to identify individuals at high risk of diabetes early on, allowing for timely intervention and personalized preventive measures. By implementing practical applications of these predictive models, healthcare providers can reduce the overall cost of healthcare spent on patients with diabetes. The project seeks to leverage the power of data-driven insights to enhance healthcare decision-making and contribute to the global effort of managing and preventing diabetes effectively. 🦠💻

## 🌟 Why diabetes? 
In 2022, CDC estimated that there were 37 million people who have diabetes, accounting for 10% of the total population in the U.S. Notably, 20% of them, approximately 7.4 million people, do not know they have the disease . The American Diabetes Association released new research in 2018 estimating the total costs of diagnosed diabetes have risen to $327 billion in 2017 . 💡💰

## 🤖 Why machine learning models?
Using machine learning models to predict the risk of developing diabetes based on patient data during their visits to medical contributes to early identification of patients and intervention of treatments, which can lead to cost savings in the long run by reducing the need for expensive treatments and hospitalizations associated with diabetes-related complications. 🤖💰

## 💰 An estimation of how machine learning models save US health care cost 
It is estimated that patients participating in the Diabetes Prevention Program can save US$1200/ patient /year . Assuming all the above-mentioned 7.4 million people who do not know they have diabetes go to clinics and get screened by machine learning models with an accuracy of 75%, a total of 5.6 million patients will be successfully identified. Assuming all of them participate in the Diabetes Prevention Program, a total of $6.72 billion will be saved per year in the U.S. 💰📊

## 📊 Details of dataset

The dataset was collected by The Behavioral Risk Factor Surveillance System (BRFSS) under the Centers for Disease Control and Prevention. BRFSS is a system of telephone surveys that collect data about U.S. residents regarding their chronic health conditions. 📊📞

## 🧹 Summary of cleaning and preprocessing

[Exploratory Data Analysis (EDA)](1_EDA_and_Data_Cleaning.ipynbnb)

Originally there were 70,692 patients’ data in the dataset, and after preprocessing steps including removing duplicates, handling missing values and handling erroneous value, there are 64,020 patients’ data left. The table shows 17 features and the target column (Diabetes).

The features can be divided into physical and behavioral features. Examples of physical features are high cholesterol and high blood pressure. Behavioral features are heavy alcohol consumption and smoker.

The target distribution, Diabetes, is approximately split evenly. This balance is desirable in machine learning applications because an imbalanced target distribution, where one class significantly outweighs the other, can lead to biased predictions and affect the model's performance.

## 📈 Let’s take a look at physical features
The probability of diabetes is significantly higher for patients with high cholesterol and high blood pressure, suggesting these two are important contributing factors to the development of diabetes. 

The probability of diabetes does not increase when the patients consume high amounts of alcohol or are smokers, suggesting that high intake of alcohol or smoking does not increase the risks of diabetes development. 📈🚭

## 📊 Insights, modeling, and results
•	The dataset was split into training and testing sets to train and evaluate the models.
•	Logistic Regression Modeling, KNN and Random Forest machine learning models were trained on the training set using the selected features and scaled data.
•	Hyperparameter tuning was performed using grid search to optimize model performance.
•	Model performance was evaluated on the testing set using various metrics, such as accuracy, precision, recall, and F1-score to assess the models' predictive capabilities. Results are summarized in the table below. 📊📈

All three models have similar accuracy levels, ranging from 0.73 to 0.75, indicating that they are making correct predictions for approximately 73% to 75% of the instances.

The recall for non-diabetes is highest for the logistic regression model (0.72), followed closely by KNN (0.69) and Random Forest (0.68). Recall is particularly important in medical contexts, as it represents the ability to correctly identify true non-diabetic cases out of all the actual non-diabetic cases.


| Model            | Accuracy | Recall (non-diabetes) |
|------------------|----------|-----------------------|
| Logistic Reg.    | 0.73     | 0.72                  |
| KNN              | 0.74     | 0.69                  |
| Random Forest    | 0.75     | 0.68                  |

## 📑 Findings and conclusions

Limitations of the dataset 
•	The dataset does not separate Type I and II diabetes
•	The dataset does not contain family history or races of patients, which are important factors for Type I diabetes

## ✅ Achieved the goal of developing machine learning models
The project's primary goal was to develop machine learning models capable of predicting the risk of developing diabetes based on patient data during medical visits. The logistic regression, KNN, and Random Forest models achieved this goal by providing predictions with relatively high accuracy (75%) and acceptable recall for non-diabetes cases.

## 💉 Practical application: Healthcare Cost Reduction
Proactive management of diabetes risk can potentially lead to reduced healthcare costs by preventing or delaying diabetes-related complications that require costly treatments and hospitalizations. As previously described, a machine learning model with an accuracy of 75% could potentially save $6.72 per year in the U.S. 💉🏥


