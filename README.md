# Mobile Reviews Sentiment Analysis and Evaluation

**Course:** CSC17104 – Programming for Data Science  
**Institution:** Faculty of Information Technology, University of Science, Vietnam National University Ho Chi Minh City  
**Academic Year:** 2025-2026

---

## Team Members

| Name | Student ID | Contribution |
|------|-----------|-------------|
| Nguyễn Huy Hoàng | 23122031 | 100% |
| Trần Tạ Quang Minh | 23122042 | 100% |
| Nguyễn Bá Nam | 23122043 | 100% |

### Work Distribution

**Nguyễn Huy Hoàng**
- Exploratory Data Analysis
- Research Questions 3, 4, and 5 formulation and analysis
- Notebook structure design

**Trần Tạ Quang Minh**
- Research Questions 5 and 6 formulation and analysis
- EDA support and data preprocessing

**Nguyễn Bá Nam**
- Research Questions 1 and 2 formulation and analysis
- Project documentation and summarization

---

## Project Overview

This project conducts a comprehensive analysis of mobile phone customer reviews to extract insights about consumer satisfaction, purchasing behavior, and sentiment patterns across different demographics and platforms. Through systematic data exploration, statistical analysis, and machine learning modeling, we investigate the factors influencing customer ratings and develop predictive models for sentiment classification.

---

## Dataset Information

### Source
- **Platform:** Kaggle
- **URL:** https://www.kaggle.com/datasets/mohankrishnathalla/mobile-reviews-sentiment-and-specification
- **Author:** Mohankrishna Thalla
- **License:** CC0: Public Domain (suitable for educational purposes)

### Dataset Characteristics
- **Size:** 50,000 rows × 25 columns
- **Scope:** Customer reviews from major e-commerce platforms (Amazon, Flipkart, AliExpress, eBay, BestBuy)
- **Geography:** Multi-country dataset covering diverse markets
- **Content:** Comprehensive mobile phone reviews including ratings, sentiment labels, review text, specifications, and demographic information

### Data Collection Method
The dataset aggregates real customer reviews from multiple e-commerce platforms across various countries, capturing authentic post-purchase experiences and evaluations from actual users.

### Data Quality
- No missing values detected
- No duplicate entries
- Clean and structured format
- Balanced representation across major mobile phone brands and price segments

---

## Research Questions

This study addresses six substantive research questions designed to extract meaningful insights from customer review data:

### Question 1: Psychology of Review Helpfulness
**Objective:** Investigate whether the community tends to trust critical reviews more than positive ones by analyzing the relationship between sentiment, review length, and helpful votes.

**Significance:** Understanding review credibility patterns helps brands identify content that influences purchasing decisions and enables better crisis management strategies.

### Question 2: E-commerce Platform Comparison
**Objective:** Determine which platforms attract premium product segments and analyze differences in customer spending patterns and purchase verification rates across platforms.

**Significance:** Provides strategic insights for manufacturers regarding optimal distribution channels and platform-specific customer behavior patterns.

### Question 3: Brand Performance and Value Assessment
**Objective:** Compare average ratings across brands, examine price-rating relationships, identify brands offering the best value for money, and analyze geographic variations in brand perception.

**Significance:** Delivers data-driven guidance for consumers making purchasing decisions and reveals competitive positioning across different markets.

### Question 4: Age-Based Preference Analysis
**Objective:** Examine how different age groups (18-25, 26-39, 40+) evaluate mobile phones differently, identifying feature priorities (battery, camera, design, performance, display) and brand preferences by demographic segment.

**Significance:** Enables targeted product development and marketing strategies tailored to specific age demographics.

### Question 5: Market Strictness Evaluation
**Objective:** Identify which geographic markets exhibit the most stringent evaluation standards by analyzing average ratings and negative review proportions across countries.

**Significance:** Helps manufacturers understand market-specific quality expectations and adjust regional strategies accordingly.

### Question 6: Sentiment Prediction Using Natural Language Processing
**Objective:** Develop and evaluate machine learning models (Multinomial Naive Bayes, Logistic Regression) to automatically classify sentiment from review text without relying on numerical ratings, and identify the most influential keywords for sentiment determination.

**Significance:** Enables automated sentiment analysis for large-scale review monitoring, customer service automation, and brand reputation management.

---

## Key Findings

### Review Interaction Behavior
Positive reviews receive significantly more "Helpful" votes compared to negative or neutral reviews. Review length does not determine helpfulness, indicating that the community values well-reasoned positive experiences over emotional criticism.

### E-commerce Platform Parity
The five major platforms (Amazon, Flipkart, AliExpress, eBay, BestBuy) demonstrate comparable price distributions and verification rates (approximately 80%), suggesting a relatively level competitive landscape in the mobile phone e-commerce market.

### Brand Performance and Value
Average ratings across brands are remarkably similar (3.11–3.14), while value-for-money metrics favor mid-range brands such as Realme, Xiaomi, and Motorola. Price shows minimal correlation with ratings, indicating that higher prices do not guarantee higher customer satisfaction.

### Demographic Preferences
The three age groups (18-25, 26-39, 40+) exhibit similar overall satisfaction levels but differ in feature priorities: younger users prioritize performance, middle-aged users emphasize camera quality, and older users focus on display and battery life.

### Geographic Evaluation Patterns
Cross-country differences in evaluation strictness are minimal (rating range approximately 0.03), with negative review proportions hovering around 20% across all markets. Geographic location is not a decisive factor in mobile phone evaluation standards.

### Natural Language Processing Results
The sentiment classification pipeline using text preprocessing, CountVectorizer, and machine learning models (Naive Bayes and Logistic Regression) achieved high accuracy on the test set. Clear emotional keywords distinguish positive from negative reviews, making automated sentiment classification practically viable.

---

## Methodology Overview

### Data Exploration
- Comprehensive statistical analysis of all 25 variables
- Distribution analysis of ratings, sentiment, price, and demographic features
- Correlation analysis between numerical variables
- Brand and platform comparative analysis
- Missing value and data quality assessment

### Data Preprocessing
- Text cleaning and normalization for review content
- Feature engineering for age groups and price segments
- Categorical variable encoding
- Train-test split for machine learning models

### Analysis Techniques
- Descriptive statistics and visualization
- Comparative analysis across brands, platforms, and demographics
- Correlation analysis
- Statistical hypothesis testing
- Natural language processing and text mining
- Machine learning classification modeling

### Machine Learning Implementation
- Text vectorization using CountVectorizer (bag-of-words with bigrams)
- Model training: Multinomial Naive Bayes and Logistic Regression
- Performance evaluation using accuracy and F1-score metrics
- Confusion matrix analysis
- Feature importance extraction through word cloud visualization

---

## Project Structure

```
p4ds-final/
├── README.md                           # Project documentation (this file)
├── Final_Project.ipynb                 # Main analysis notebook
├── Mobile Reviews Sentiment.csv        # Dataset
└── references/                        # Additional reference materials
```

---

## Technical Requirements

### Programming Language
- Python 3.8+

### Core Libraries
- **Data Manipulation:** pandas, numpy
- **Visualization:** matplotlib, seaborn
- **Text Processing:** nltk, wordcloud
- **Machine Learning:** scikit-learn
- **Statistical Analysis:** scipy

### Execution Instructions

1. Ensure all required libraries are installed
2. Place the dataset file `Mobile Reviews Sentiment.csv` in the project directory
3. Open `Final_Project.ipynb` in Jupyter Notebook or JupyterLab
4. Execute cells sequentially from top to bottom
5. All visualizations and results will be generated inline

---

## Limitations and Constraints

### Data Source Limitations
- Dataset collected from Kaggle may not comprehensively represent the entire mobile phone market
- Potential selection bias toward users motivated to write reviews
- Limited temporal coverage preventing longitudinal trend analysis

### Scope Limitations
- Analysis focused on major platforms and countries, excluding emerging markets and offline channels
- Missing contextual variables such as income levels, detailed usage patterns, and device usage duration
- Conclusions are indicative rather than universally generalizable

### Model Limitations
- Exceptionally high model performance may indicate data leakage or synthetic data characteristics
- Limited to traditional machine learning models without exploring advanced embedding techniques
- Requires validation on external datasets to confirm generalization capability

---

## Future Directions

### Data Enhancement
- Integrate additional data sources including social media, forums, and independent review websites
- Incorporate detailed demographic and economic indicators for deeper customer segmentation
- Expand geographic coverage to include emerging markets

### Advanced Modeling
- Implement modern NLP architectures including TF-IDF with SVM, Bi-LSTM, and Transformer models (BERT)
- Conduct comprehensive hyperparameter tuning and cross-validation
- Develop multi-metric evaluation frameworks including ROC curves and class-specific performance analysis

### Temporal Analysis
- Convert review dates to datetime format for time-series analysis
- Investigate sentiment trends over time, particularly around product launches and major events
- Analyze seasonal patterns in review behavior and ratings

### Applied Systems
- Develop recommendation systems based on user preferences and demographic profiles
- Create real-time sentiment monitoring dashboards for brand management
- Build decision support tools for consumers and manufacturers

---

## Conclusions

This project demonstrates the application of data science methodologies to extract actionable insights from customer review data. Through systematic exploration, rigorous analysis, and machine learning modeling, we have uncovered patterns in consumer behavior, brand performance, and sentiment dynamics that hold practical value for both consumers and industry stakeholders. The findings challenge common assumptions about review credibility, brand-price relationships, and market differences while confirming the viability of automated sentiment analysis for large-scale application.

The integration of statistical analysis with natural language processing showcases the multidisciplinary nature of modern data science and highlights the importance of combining quantitative rigor with practical business understanding.

---

## Acknowledgments

We express our sincere gratitude to the instructors of CSC17104 for their guidance throughout this project and for providing a comprehensive framework for conducting data science research. This project has significantly enhanced our understanding of the complete data science workflow and prepared us for future analytical challenges.

---

**Project Completion Date:** December 2025  
**Repository:** Vietnam National University, Ho Chi Minh City - University of Science
