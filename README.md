# Health Insurance Analysis
## Table of Contents


- [Project Overview]( #Project-Overview)
- [Data Sources](#Data-Sources)
- [Tools ](Tools)
- [Data Cleaning and Pre-processing](#Data-Cleaning-and-Pre-processing)
- [Analysis ](Analysis)
- [Findings ](Findings)
-  [Recommendation ](Recommendations)
- [Limitations ](Limitations)
- [REFERENCES](REFERENCES)
<img width="1003" alt="correlation matrix" src="https://github.com/user-attachments/assets/9fadba35-5efc-406d-80d8-d1ecb28d96e2">

### Project Overview
This document details the analysis of a medical insurance dataset to predict insurance charges based on various features. The analysis highlights how different factors impact insurance costs.

### Data Sources
The primary dataset used is insurance.csv, which contains information on individuals and their insurance charges.

### Tools
Python: For data cleaning, analysis, and prediction
Libraries: pandas, seaborn, matplotlib, scikit-learn
  
### Data Cleaning and Pre-processing

- Data Loading and Overview: Loaded the dataset and displayed initial and summary statistics.
- Checking and Handling Missing Values: Checked for and addressed missing values.
- Data Cleaning and Formatting: Converted categorical columns to numerical values for analysis.
- Feature Reduction and Normalization: Applied transformations to prepare data for modeling.

### Analysis
The dataset was analyzed using a linear regression model to predict insurance charges. Key steps included:

'''python
Code
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression

# Train/Test Split
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

# Model Training
lr = LinearRegression()
lr.fit(X_train, y_train)'''

### Results
The linear regression model revealed a significant difference in predicted insurance charges between smokers and non-smokers. Specifically:

Smokers: Predicted insurance cost was £36,751.18.
Non-Smokers: Predicted insurance cost was £13,115.28.
This demonstrates a strong correlation between smoking status and insurance charges, with smokers facing much higher premiums.

### Recommendation

The analysis  used few features, which provided useful insights, but expanding the feature set could enhance the model's accuracy.
Having a dataset with additional variables such as occupation, education level, geographic data, health history, and lifestyle factors may uncover deeper correlations and improve predictions. This broader approach could better capture variations in insurance costs and provide more precise predictions.

### Limitations
The analysis relied on a linear regression model, which may not have captured all complexities of the data. 

