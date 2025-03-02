# AB_Tests
AB/Test
# A/B Test with AI 🚀  

This repository contains a Python-based A/B testing script enhanced with AI for predicting RPM.  

## 📊 Features  
- Calculates key performance metrics (RPM, RPS, CTR)  
- Performs statistical hypothesis testing  
- Visualizes A/B test results using Seaborn  
- Uses Random Forest to predict RPM  
# 📊 AI-Driven A/B Testing Analysis

## 🔍 Project Overview
This project analyzes an A/B test conducted on **Marketpele Feed**, a platform that helps publishers monetize through advertisements. The experiment compares two different placements of paid and organic content to determine their impact on key metrics.

## 🧪 Experiment Details
- **Group A**: Organic element at the top, followed by four paid elements.
- **Group B**: Four paid elements at the top, followed by one organic element.

## 🎯 Key Metrics Analyzed
- **RPM** (Revenue per 1000 impressions)
- **RPS** (Revenue per session)
- **Paid CTR** (Click-through rate on ads)
- **Organic CTR** (Click-through rate on organic content)

## 📊 Statistical Analysis & Results
- Conducted **t-tests** to check if differences are statistically significant.
- Found that **Paid CTR significantly increased** in Group B.
- **Organic CTR significantly decreased** in Group B.
- **Revenue-related metrics (RPM, RPS) did not show significant differences.**

## 🤖 AI Model for Revenue Prediction
A **Random Forest Regressor** was trained to predict RPM based on:
- Pageviews, visible pageviews, sessions
- Sponsored (paid) clicks, organic clicks
- A/B group as a feature

**Mean Absolute Error (MAE) of prediction**: ~0.94 RPM

## 🚀 How to Run This Project
### In Google Colab:
1. Upload `marketpele_ab_test.xlsx` to Colab.
2. Clone this repo:
   ```sh
   !git clone https://github.com/yourusername/AB_Testing_AI_Analysis.git
   ```
3. Open and run `ab_test_ai_analysis.py` in Colab.

### Locally:
1. Install dependencies:
   ```sh
   pip install pandas numpy seaborn scikit-learn scipy matplotlib
   ```
2. Run the script:
   ```sh
   python ab_test_ai_analysis.py
   ```

## 📂 Files in This Repository
- `ab_test_ai_analysis.py` → Python script for data analysis and AI model
- `marketpele_ab_test.xlsx` → Dataset used for A/B testing
- `ab_test_model.pkl` → Trained AI model for revenue prediction
- `README.md` → Project documentation

## 📢 Conclusion
This analysis shows that moving paid elements to the top **increases ad clicks** but reduces organic engagement. AI modeling helps forecast potential long-term revenue impact, guiding better business decisions.

---
📌 **Author**: [Aaliyah]  




