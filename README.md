# Customer Subscription Prediction Analysis

> Comprehensive machine learning classification project comparing 5 different algorithms to predict customer subscription behaviour using KNIME Analytics Platform

## 🎯 Project Overview

This project tackles the business-critical challenge of predicting whether customers will subscribe to a service based on historical marketing data. Using KNIME Analytics Platform, I implemented and compared five classification algorithms to identify the optimal approach for customer targeting and marketing strategy optimization.

**Key Achievement:** Random Forest model achieved **96% validation accuracy** and secured **top 15% placement** in Kaggle competition (0.62658 score)

## 📊 Dataset Information

- **Training Data:** 26,360 customer records with 23 features
- **Test Data:** 6,590 records for Kaggle submission
- **Target Variable:** Binary subscription status (0/1)
- **Challenge:** Highly imbalanced dataset (89% non-subscribers)

### Key Features
- **Demographics:** Age, job, marital status, education
- **Financial:** Default status, housing loans, personal loans
- **Campaign:** Contact method, duration, previous campaigns
- **Economic:** Employment rate, consumer confidence, interest rates

## 🛠️ Technical Implementation

### Data Preprocessing Pipeline
- **Missing Value Handling:** Imputation using most frequent (categorical) and median (numerical)
- **Class Imbalancing:** SMOTE technique to balance 89%/11% distribution
- **Feature Engineering:** Category to number conversion, normalization
- **Data Splitting:** 70/30 train/validation with consistent random seed

### Machine Learning Models Implemented

| Algorithm | Validation Accuracy | Precision | Recall | F1-Score | AUC |
|-----------|-------------------|-----------|---------|----------|-----|
| **Random Forest** | **96%** | **94%** | **99%** | **96%** | **99%** |
| Decision Tree | 92% | 89% | 94% | 92% | 95% |
| K-Nearest Neighbours | 92% | 90% | 94% | 92% | 95% |
| Neural Network (MLP) | 86% | 81% | 94% | 87% | 91% |
| Support Vector Machine | 89% | 89% | 0% | 94% | 50% |

## 🔧 KNIME Workflow Architecture

### Core Pipeline Components
1. **Data Import & Type Casting**
2. **Missing Value Treatment**
3. **SMOTE Balancing**
4. **Feature Preprocessing**
5. **Model Training & Validation**
6. **Performance Evaluation**
7. **Kaggle Submission Export**

### Advanced Features
- **Parameter Optimization Loops** for hyperparameter tuning
- **ROC Curve Analysis** for model performance assessment
- **Feature Importance Analysis** using Random Forest attribute statistics
- **Cross-Validation** for robust model evaluation

## 📈 Key Results & Insights

### Best Performing Model: Random Forest
- **Training Accuracy:** 99.8%
- **Validation Accuracy:** 96%
- **Kaggle Score:** 0.62658 (Top 25%)
- **Key Strength:** Excellent balance of precision and recall

### Feature Importance Findings
Random Forest attribute statistics revealed the most predictive features for subscription behaviour, enabling targeted marketing strategies.

### Business Impact
- **96% accuracy** enables confident customer targeting
- **Reduced marketing costs** through precise subscriber identification
- **Improved ROI** on marketing campaigns through data-driven decisions

## 🚀 Technical Skills Demonstrated

### Machine Learning
- **Classification Algorithms:** Decision Trees, Random Forest, KNN, SVM, Neural Networks
- **Model Evaluation:** ROC/AUC analysis, confusion matrices, cross-validation
- **Hyperparameter Tuning:** Grid search and optimization loops
- **Class Imbalancing:** SMOTE implementation for skewed datasets

### Data Science Pipeline
- **Data Preprocessing:** Missing value treatment, feature scaling, encoding
- **Feature Engineering:** Category conversion, normalization techniques
- **Model Comparison:** Systematic evaluation across multiple algorithms
- **Performance Optimization:** Parameter tuning for each algorithm

### Tools & Technologies
- **Primary Platform:** KNIME Analytics Platform
- **Competition:** Kaggle submission and leaderboard participation
- **Visualization:** ROC curves, confusion matrices, performance charts
- **Documentation:** Comprehensive analysis and methodology reporting

## 📁 Repository Structure

```
customer-subscription-prediction/
├── data/
│   ├── Assignment3UnknownDataset.csv (test data)
│   ├── Assignment3MarketingDataset.csv (training data)
│   └── sample_predictions.csv (Kaggle submission)
├── docs/
│   └── full_analysis_report.pdf
├── results/
│   └── model_performance_comparison.png
├── workflows/
│   ├── Decision_tree_workflow.png
│   ├── K_nearest_neighbour_workflow.png
│   └── neural_network_workflow.png
│   ├── random_forest_workflow.png
│   ├── svm_optimization_workflow.png
├── README.md
```

## 🎯 Business Applications

This analysis directly applies to:
- **Customer Acquisition:** Identify high-probability prospects
- **Marketing Optimization:** Allocate budget to most promising segments
- **Campaign Targeting:** Personalize outreach based on prediction confidence
- **Resource Planning:** Forecast subscription volumes for capacity planning

## 🔍 Future Enhancements

- **Deep Learning:** Implement advanced neural architectures
- **Ensemble Methods:** Combine top-performing models
- **Real-time Prediction:** Deploy model for live customer scoring
- **Feature Engineering:** Create interaction terms and polynomial features

## 📧 Contact

**Zyad Kamal Hamed**  
📧 zyad2408@live.com.au  
🔗 [LinkedIn](https://linkedin.com/in/zyadkamalhamed/)  

---
*Demonstrating end-to-end machine learning capabilities from data preprocessing to model deployment and business impact*
