<body>
    <h1>Impact of Gaming Habits and Demographics on Mental Health</h1>
</body>


# Gaming Habits and Mental Health Analysis

## Overview
This project analyzes the relationship between gaming habits, demographics, and mental health outcomes using machine learning approaches. The study utilizes a comprehensive dataset from the Open Source Framework (OSF) containing information about gamers' psychological metrics and demographic data.

## Key Features
- Analyzes three mental health indicators:
  - General Anxiety Disorder (GAD)
  - Satisfaction with Life (SWL)
  - Social Phobia Inventory (SPIN)
- Implements two machine learning models:
  - Random Forest Classifier
  - Support Vector Machine (SVM) with polynomial kernel
- Uses Principal Component Analysis (PCA) for dimensionality reduction
- Includes custom evaluation metrics for multi-class classification

## Data Processing
- Initial dataset: 13,464 rows × 55 columns
- Cleaned and preprocessed data by removing irrelevant columns and handling missing values
- Encoded categorical variables using one-hot encoding and label encoding
- Reduced dimensions using PCA while preserving data integrity

## Model Performance
### Random Forest
- Best performing model with 35% accuracy on GAD_T
- Average distance from true class: 2.58 (compared to random guess of 20.7)
- 86.30% of predictions within 2 classes of true GAD_T score

### SVM
- Improved using OneVsRestClassifier approach
- Performance after optimization:
  - GAD_T: 24.71%
  - SWL_T: 13.50%
  - SPIN_T: 7.48%
- Average distance from true class: 5.52

## Technologies Used
- Python
- Libraries:
  - Pandas
  - Seaborn
  - Matplotlib
  - NumPy
  - Scikit-learn
- Jupyter Notebook

## Future Work
- Incorporate rank standardization across different games
- Analyze correlation between rank and stress levels
- Study the transition from casual to competitive gaming
- Investigate relationship between gaming skill ceiling and stress indicators

## References
1. M. Sauter and D. Draschkow, "Gaming Habits and Psychological Well-being" (OSF, 2017)
2. M. Kowal et al., "Gaming Your Mental Health" (JMIR Publications, 2021)
3. James McClellan Smith, "The Relationship Between Video Game Use and Couple Attachment Behaviors" (BYU, 2013)
4. S. Park et al., "Measurement of craving among gamers" (BMC Public Health, 2023)
