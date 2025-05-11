# CodeAlpha Tasks

## TASK 1: Titanic Classification Project

This project involves predicting the survival of passengers aboard the Titanic using various machine learning techniques. The dataset used contains information about passengers, such as their age, gender, class, and embarkation location. The goal is to classify whether each passenger survived or not.

### Key Steps
**1. Data Preprocessing**

The dataset was cleaned by removing irrelevant columns (PassengerId, Ticket, Cabin).

Missing values were handled by filling the 'Age' column with the median and the 'Embarked' column with the mode.

Duplicate entries were checked and removed.

A new feature, Title, was extracted from the Name column, which was then replaced with common titles like "Miss," "Mrs.," and "Mr."

Additional features like FamilySize and IsAlone were created to aid in classification.

**2. Feature Engineering**

Categorical variables were one-hot encoded, and numeric variables were scaled using StandardScaler.

Key features included Pclass, Sex, Age, Fare, Embarked, and the new Title and IsAlone.

**3. Model Training**

An XGBoost classifier was used as the model, implemented in a pipeline with preprocessing steps.

The data was split into training and testing sets (80/20 ratio).

The model was evaluated using accuracy, classification report, and confusion matrix.

**4. Model Evaluation**

The model achieved good accuracy, with the confusion matrix and classification report indicating solid performance.

Visualizations were created to showcase survival rates across different groups (e.g., by sex, class, and age).

### Insights

Gender: Females had a significantly higher survival rate, especially in 1st class.

Class: Passengers in 1st class had a much higher survival rate compared to those in 2nd and 3rd classes.

Age: Children and young adults had a better chance of survival, with children under 12 having the highest survival rate.

Embarked Location: Passengers who embarked from Cherbourg (C) had the highest survival rate.

Family Size: Passengers traveling alone had a lower survival rate compared to those with family.

### Conclusion

This analysis highlights key trends and factors that influenced survival on the Titanic. The model successfully predicted survival with high accuracy, providing insights into which features were most significant.
