# 📊 Students Performance Analysis
This project explores a real-world dataset of 5,000 students to uncover patterns, correlations, and factors affecting academic performance. It involves detailed Exploratory Data Analysis (EDA), data cleaning, visualization, and preprocessing — laying the groundwork for predictive modeling.

## Project Goals
- Understand key factors influencing student performance.
- Analyze relationships between demographic, academic, and behavioral features.
- Handle missing values and prepare the dataset for machine learning models.
- Provide data-driven insights for potential educational interventions.

## Dataset Overview
- **Source**: [Kaggle: Students Grading Dataset](https://www.kaggle.com/datasets/mahmoudelhemaly/students-grading-dataset)
- **Records**: 5,000 students
- **Format**: CSV

## Features Summary
- **Identifiers**: `Student_ID`, `First_Name`, `Last_Name`, `Email`
- **Demographics**: `Gender`, `Age`, `Department`, `Parent_Education_Level`, `Family_Income_Level`
- **Academic Performance**: `Attendance (%)`, `Midterm_Score`, `Final_Score`, `Assignments_Avg`, `Quizzes_Avg`, `Participation_Score`, `Projects_Score`, `Total_Score`, `Grade`
- **Behavioral Factors**: `Study_Hours_per_Week`, `Stress_Level`, `Sleep_Hours_per_Night`, `Extracurricular_Activities`, `Internet_Access_at_Home`

## Notebook Flow
The notebook follows a clear, structured analysis pipeline:

1. **Import Libraries & Load Data**  
   Import essential libraries (Pandas, NumPy, Seaborn, etc.) and load the dataset.

2. **Initial Exploration**  
   View dataset shape, feature types, and detect null values.

3. **Data Cleaning & Missing Value Handling**  
   - Apply KNN imputation for numerical features.
   - Assign "Unknown" category for missing categorical values.

4. **Univariate Analysis**  
   - Visualize distributions of numerical features (histograms, boxplots).
   - Analyze frequency counts for categorical features (bar plots).

5. **Multivariate Analysis**  
   - Use scatter plots and bar plots to explore relationships.
   - Correlation heatmaps to detect relationships between academic scores.
   - Perform statistical tests:
     - **Chi-Square Test** for categorical dependencies.
     - **Spearman Correlation** for non-linear numerical relations.
     - **ANOVA** for group mean comparison.

6. **Key Findings Summary**  
   Highlight the most significant insights from the analysis.

7. **Data Preprocessing for Modeling**  
   - Encode categorical variables (Ordinal + One-Hot).
   - Normalize numerical features using Min-Max Scaling.
   - Split data into training and testing sets (80/20 split).

## Techniques Used
- Data Cleaning (KNN Imputation, Missing Value Handling)
- Univariate & Multivariate Analysis (Histograms, Boxplots, Correlation Heatmaps)
- Statistical Testing (Chi-Square, ANOVA, Spearman)
- Feature Encoding (Ordinal, One-Hot)
- Scaling (Min-Max Normalization)
- Train-Test Split (80/20)

## Key Findings
- Attendance alone does not strongly predict academic success.
- Quality of study is more impactful than quantity.
- Participation score and performance do not always correlate positively.
- Demographics like gender and income have minimal impact on scores.


