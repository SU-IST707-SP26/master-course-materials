# Lecture Topic Overview: Advanced Data Preparation

## Learning Objectives
Students will be able to:
- Identify and handle outliers using visual, statistical, and machine learning approaches
- Select appropriate scaling techniques based on data distribution characteristics
- Implement advanced imputation strategies for missing data beyond simple replacement methods
- Choose optimal encoding strategies for categorical variables with different characteristics  
- Diagnose and address class imbalance using resampling and algorithmic techniques
- Build robust preprocessing pipelines that handle real-world data quality issues systematically
- Understand the impact of preprocessing choices on downstream model performance
- Create custom transformers for specialized preprocessing needs

## Topics Covered
**Outlier Detection and Handling:**
- Visual detection methods: box plots, scatter plots, histograms for univariate and bivariate analysis
- Statistical methods: Z-score and IQR (Interquartile Range) approaches
- Advanced ML-based detection: IsolationForest, EllipticEnvelope, Local Outlier Factor (LOF), One-Class SVM
- Handling strategies: removal, winsorizing, transformation (log, Box-Cox), robust methods
- Custom outlier removal transformers for pipeline integration

**Data Scaling and Normalization:**
- Understanding when scaling is critical (distance-based algorithms, neural networks)
- StandardScaler for normally distributed data
- MinMaxScaler for bounded distributions
- RobustScaler for outlier-resistant scaling using median and IQR
- Handling different distribution types (normal vs. power-law distributions)
- Impact of scaling choice on algorithm performance

**Missing Data Analysis and Imputation:**
- Types of missingness: Missing Completely at Random (MCAR), Missing at Random (MAR), Missing Not at Random (MNAR)
- Simple imputation approaches and their limitations
- Advanced imputation techniques:
  - Multiple Imputation by Chained Equations (MICE)
  - K-Nearest Neighbors (KNN) imputation
  - Iterative imputation strategies
- Comparing imputation method effectiveness

**Categorical Data Encoding:**
- Ordinal encoding for naturally ordered categories
- One-hot encoding and its computational trade-offs
- Handling high-cardinality categorical features
- Target encoding techniques and overfitting prevention
- Binary encoding for memory efficiency
- Feature hashing for extremely high cardinality

**Class Imbalance Management:**
- Detection and quantification of imbalanced datasets
- Resampling techniques:
  - SMOTE (Synthetic Minority Oversampling Technique)
  - Strategic undersampling approaches
  - Combination methods
- Algorithmic approaches: cost-sensitive learning
- Evaluation considerations for imbalanced data scenarios

## Practical Skills
After completing this section, students can:
- Diagnose data quality issues systematically
- Implement appropriate preprocessing strategies for different data types and distributions
- Build custom transformers following scikit-learn conventions
- Create preprocessing pipelines that handle complex real-world data scenarios
- Evaluate the impact of preprocessing decisions on model performance
- Handle missing data appropriately based on missingness mechanisms
- Address class imbalance effectively using multiple strategies

## Prerequisites
- Lecture 02: Basic data preparation and scikit-learn pipelines
- Understanding of basic statistical concepts (mean, median, quartiles, standard deviation)
- Familiarity with scikit-learn transformer API

## Key Materials
**Core Notebooks:**
- `1-outliers.ipynb`: Visual, statistical, and ML-based outlier detection with custom transformer implementation
- `2-scaling.ipynb`: Comprehensive scaling methods with distribution-specific recommendations
- `3-missingness-imputation.ipynb`: Basic missing data handling and simple imputation approaches
- `4-encoding.ipynb`: Categorical encoding strategies with high-cardinality examples
- `5-imputation-redux.ipynb`: Advanced imputation techniques including MICE and KNN methods
- `6-imbalanced-classes.ipynb`: Class imbalance detection and correction using multiple approaches

**Supporting Materials:**
- `data/sample_data_with_outliers.csv`: Synthetic dataset for outlier detection practice
- `data/synthetic_patient_data.csv`: Medical dataset with missing values for imputation practice
- `data/synthetic_patient_data_unbalanced.csv`: Imbalanced dataset for resampling techniques
- `assets/MICE.png`: Multiple imputation visualization aid
- `extra/`: Advanced topics including cross-validation with tuning and regression evaluation

## Time Estimate
- Outlier detection and handling: 3-4 hours
- Scaling techniques: 2-3 hours
- Missing data imputation: 4-5 hours
- Categorical encoding: 2-3 hours
- Class imbalance: 3-4 hours
- **Total: 14-19 hours**

## Assessment Preparation
This section prepares students for:
- Real-world data preprocessing challenges in assignments
- Advanced preprocessing pipeline construction
- Data quality assessment and remediation
- Preprocessing strategy justification in project reports
- Performance impact analysis of preprocessing choices