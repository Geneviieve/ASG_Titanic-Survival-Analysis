# ASG-Titanic-Survival-Analysis
Introductory case study on data analysis and preprocessing using the classic Titanic dataset.


This repository documents a preliminary assignment in data analysis, completed as part of a Machine Learning course.

The objective of this exercise is to practice the foundational data science workflow, from data cleaning and preprocessing to exploratory data analysis on the classic Titanic dataset. This case study serves as a fundamental introduction to handling a real-world dataset before applying machine learning models. The dataset used is the famous "Titanic: Machine Learning from Disaster" from Kaggle. The objective is to analyze the factors that strongly correlate with a passenger's chance of survival.

## Analysis Process
The analysis in the notebook follows standard data preprocessing steps:
    
    - Data Cleaning:
        Filled missing values in the Age column with the median value.
        Filled missing values in the Embarked column with the mode (the most frequent value).
        Dropped the Cabin column due to a high number of missing values.

    - Feature Selection:
        Removed columns irrelevant to the analysis, such as PassengerId and Name.

    - Data Transformation:
        Label Encoding: Converted the categorical Sex feature (male/female) into numerical values (0/1).
        Normalization: Scaled the values in the Age column to a 0-1 range using MinMaxScaler to prevent it from dominating other features.

    - Data Visualization:
        Created various plots (histograms, bar charts) to visualize data distributions and the relationships between variables, particularly in relation to the Survived target variable.

## Key Findings (Insights)
The visualizations led to several key insights:

    Survival Rate by Passenger Class: First-class passengers had a significantly higher survival rate compared to second and third-class passengers. This suggests that socio-economic status played a critical role.
    Survival Rate by Sex: Female passengers had a much higher survival rate than male passengers, likely due to the "women and children first" evacuation policy.
    Survival Rate by Age: Children had a better chance of survival, while middle-aged passengers accounted for the largest number of fatalities, reinforcing the hypothesis of an evacuation priority for the young.

## Tools Used
- Python
- Pandas: for data manipulation and analysis.
- Matplotlib & Seaborn: for data visualization.
- Scikit-learn: for data preprocessing (LabelEncoder, MinMaxScaler).
- Jupyter Notebook as the working environment.
