# Project Problem Statement

The rising prevalence of diabetes is posing significant challenges to healthcare systems in the U.S., leading to substantial healthcare expenditures. To address this issue and mitigate the burden on healthcare costs, the project aims to develop and deploy machine learning models that can accurately predict the risk of developing diabetes based on readily available health datasets. The objective is to identify individuals at high risk of diabetes early on, allowing for timely intervention and personalized preventive measures. By implementing practical applications of these predictive models, healthcare providers can reduce the overall cost of healthcare spent on patients with diabetes. The project seeks to leverage the power of data-driven insights to enhance healthcare decision-making and contribute to the global effort of managing and preventing diabetes effectively.

## Why Diabetes?

In 2022, the CDC estimated that there were 37 million people with diabetes, accounting for 10% of the total U.S. population. Shockingly, 20% of them—approximately 7.4 million people—remain unaware of their condition. The American Diabetes Association reported a 26% increase in the total costs of diagnosed diabetes from 2012 to 2017, reaching $327 billion in 2017. Moreover, a staggering $1 out of every $4 in U.S. healthcare costs is spent on caring for people with diabetes.

## Why Machine Learning Models?

Using machine learning models to predict diabetes risk based on patient data during medical visits facilitates early patient identification and intervention, ultimately reducing the need for costly treatments and hospitalizations associated with diabetes-related complications.

## Machine Learning Models' Potential to Save Healthcare Costs

If all the 7.4 million people unaware of their diabetes risk were screened with machine learning models, assuming an accuracy of 75%, it could save $6.72 billion annually in the U.S.

## Details of the Dataset

The dataset was collected by The Behavioral Risk Factor Surveillance System (BRFSS) under the Centers for Disease Control and Prevention.

## Summary of Cleaning and Preprocessing

After preprocessing, 64,020 patients' data were retained from an initial 70,692. The dataset includes 17 features and the target column (Diabetes).

## Insights, Modeling, and Results

- The dataset was split into training and testing sets.
- Logistic Regression, KNN, and Random Forest models were trained and optimized.
- Model performance metrics were evaluated and summarized in the table below.

| Model            | Accuracy | Recall (non-diabetes) |
|------------------|----------|-----------------------|
| Logistic Reg.    | 0.73     | 0.72                  |
| KNN              | 0.74     | 0.69                  |
| Random Forest    | 0.75     | 0.68                  |

## Findings and Conclusions

### Limitations of the Dataset

- The dataset does not distinguish between Type I and II diabetes.
- Family history and patient races, essential factors for Type I diabetes, are missing.

### Achieved Goals and Practical Application

The project successfully developed machine learning models to predict diabetes risk. These models achieved high accuracy (75%) and reasonable recall for non-diabetes cases. Proactively managing diabetes risk can lead to substantial healthcare cost savings, potentially saving billions annually in the U.S.
