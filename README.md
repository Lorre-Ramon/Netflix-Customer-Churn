# Netflix Customer Churn Analysis

## Overview
This project conducts an Exploratory Data Analysis (EDA) on Netflix customer churn, actively utilizing machine learning for predictive insights to understand what drives customer churn and provide actionable recommendations for retention strategies.

## Dataset
- **Source**: [Kaggle-Netflix Customer Churn dataset](https://www.kaggle.com/datasets/abdulwadood11220/netflix-customer-churn-dataset)
- **Size**: 5,000 customers
- **Features**: User demographics, user behavior, and product information

## Key Findings & Insights

### 🎯 Primary Discovery: Engagement is Everything
**Customer churn is primarily driven by user engagement metrics, not demographics or subscription type.**

1. **`avg_watch_time_per_day`** - Explains ~40% of churn variance
2. **`watch_hours`** - Total viewing time
3. **`last_login_days`** - Recency of platform usage

**Combined Impact**: These three features explain ~86% of the variance in customer churn behavior.

### 📊 Feature Importance Analysis
- **High Impact**: Engagement metrics (watch time, login frequency)
- **Low Impact**: Demographics (age, gender, region) and subscription type
- **Insight**: Netflix retention is behavior-driven, not product-tier driven

### 🔍 Model Performance
- **Random Forest**: ~92% accuracy in predicting customer churn
- **Logistic Regression**: ~89% accuracy in predicting customer churn with better interpretability
- **ROC Analysis**: Both models show strong discriminative power (AUC > 0.9)

## Machine Learning Approach

### Data Preprocessing
- **Categorical Encoding**: One-hot encoding for categorical features
- **Feature Scaling**: StandardScaler for continuous variables
- **Feature Engineering**: Age bucketing and correlation analysis

### Cross-Validation Results (for Logistic Regression)
- Stable performance across different data splits
- Minimal overfitting detected
- Strong generalization capability

### Model Comparison
| Model | Accuracy | AUC | Key Strengths |
|-------|----------|-----|---------------|
| Random Forest | ~92% | 0.98 | Feature importance insights |
| Logistic Regression | ~89% | 0.96 | Interpretable coefficients |

## Actionable Items

### 🎬 Content & Engagement Strategy
1. **Improve Content Quality**
   - Invest in high-quality original content
   - Acquire popular shows and movies
   - Focus on content that drives binge-watching behavior

2. **Enhance User Experience**
   - Optimize user interface for content discovery
   - Improve platform navigation and visual appeal
   - Reduce friction in content consumption

3. **Advanced Recommendation System**
   - Implement personalized recommendation algorithms
   - Use viewing history and preferences for better content matching
   - Increase content discovery and engagement

### 📈 Monitoring & Early Warning System
1. **Key Performance Indicators (KPIs)**
   - Monitor `avg_watch_time_per_day` trends
   - Track `watch_hours` patterns
   - Alert on `last_login_days` increases

2. **Predictive Dashboard**
   - Real-time churn risk scoring
   - User engagement trend analysis
   - Early intervention triggers

### 🎯 Retention Interventions
1. **Content Personalization**
   - Personalized content recommendations
   - Content alerts for favorite genres/actors
   - Exclusive previews for at-risk users

2. Re-Engagement & Retention
   - Re-engagement campaigns for inactive users
   - Special offers for users showing declining engagement

1. Communication & Notifications
   - Personalized notifications based on viewing history

## Conclusions

1. **Engagement Over Everything**: User engagement metrics are the strongest predictors of churn, significantly outweighing demographic or subscription factors.

2. **Predictable Patterns**: Customer churn can be predicted with ~90% accuracy using engagement-based features.

3. **Actionable Intelligence**: The analysis provides clear, data-driven recommendations focusing on content quality and user engagement rather than pricing strategies.

4. **Business Impact**: Netflix should prioritize user engagement initiatives over demographic targeting or subscription tier modifications for churn reduction.

---
*This analysis demonstrates that in the streaming industry, content engagement is the ultimate retention driver.*
