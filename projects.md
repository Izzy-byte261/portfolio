---
layout: page
title: Projects
permalink: /projects/
---

## 📂 Project Portfolio
Below are my representative projects covering machine learning, data analytics, and business analysis.

---

### Project 1: Q-Learning Based Tic-Tac-Toe AI Game
**Individual Project** | 2026.02 - 2026.03

**Problem**: Traditional Tic-Tac-Toe AI usually relies on fixed rules and lacks learning ability and challenge. This project aims to train an AI opponent that can autonomously learn optimal strategies through reinforcement learning, providing players with a more competitive gaming experience.

**Data**: No external dataset. Training data was generated through AI self-play. A total of 100,000 self-play games were conducted, generating a Q-table with 8,052 state-action pairs.

**Approach**: Implemented the standard Q-Learning algorithm, designed an ε-greedy exploration strategy, delayed reward backpropagation mechanism, and a reasonable reward function. Adopted a dual-AI self-play training mode where two independent Q-Learning agents compete against each other to learn.

**Outcome & Impact**:
- The trained AI achieved near-optimal strategy, with the draw rate increasing from 15.1% to 66.0%, aligning with the theoretical optimal outcome of Tic-Tac-Toe
- The first-mover advantage significantly diminished, with X's win rate dropping from 56.3% to 23.8%
- Developed a complete graphical user interface supporting 10-game series, real-time Q-value display, and Q-table save/load functionality

**Personal Contribution**: Independently completed algorithm design, code implementation, UI development, and project documentation

**Project Links**:
- GitHub: [https://github.com/Izzy-byte261/tic_tac_toe_qlearning](sslocal://flow/file_open?url=https%3A%2F%2Fgithub.com%2FIzzy-byte261%2Ftic_tac_toe_qlearning&flow_extra=eyJsaW5rX3R5cGUiOiJjb2RlX2ludGVycHJldGVyIn0=)
- Demo Video: [https://youtu.be/NVHrlGJrwjI](sslocal://flow/file_open?url=https%3A%2F%2Fyoutu.be%2FNVHrlGJrwjI&flow_extra=eyJsaW5rX3R5cGUiOiJjb2RlX2ludGVycHJldGVyIn0=)

---

### Project 2: Credit Card Fraud Detection Using Machine Learning
**Group Project (Team Lays, 6 members)** | 2026.02 - 2026.03
**My Role**: Lead Model Selection & Training 

**Problem**: Credit card fraud causes billions in annual losses globally. The core challenge is extreme class imbalance (only 0.17% of transactions are fraudulent), which makes standard models biased toward predicting normal transactions and fail to detect fraud cases effectively.

**Data**: Used the public Kaggle Credit Card Fraud Dataset containing 284,807 European credit card transactions over 2 days. After removing 1,081 duplicates, the cleaned dataset has 283,726 samples (283,253 normal, 473 fraudulent) with 30 numerical features (28 PCA anonymized features + Time + Amount).

**Approach (My Core Responsibility)**:
1.  **Model Selection**: Selected Logistic Regression (baseline, high interpretability) and XGBoost (high-performance ensemble model) for comparison, balancing interpretability requirements in financial risk control and predictive performance
2.  **Algorithm Implementation**: Built both models from scratch using scikit-learn and XGBoost libraries, with L2 regularization to prevent overfitting
3.  **Training Pipeline**: Designed a standardized training workflow using 5-fold cross-validation to ensure result reproducibility and avoid overfitting
4.  **Hyperparameter Tuning**: Performed grid search to optimize key parameters:
    - Logistic Regression: Tuned regularization parameter C (range: 0.01-100), optimal value C=10
    - XGBoost: Tuned learning rate (0.05-0.1) and max tree depth (3-5), optimal values: learning_rate=0.1, max_depth=5
5.  **Model Export**: Saved trained models as .pkl files for downstream validation and deployment

**Outcome & Impact**:
- XGBoost outperformed Logistic Regression across all key metrics, achieving 83% fraud recall (only 17% of fraud cases missed) and 0.98 AUC-ROC
- SMOTE oversampling improved XGBoost's F1-score by 32.1% (from 0.28 to 0.37), proving its effectiveness in addressing class imbalance
- The final model reduced false positive alarms by 83% compared to the baseline Logistic Regression, significantly lowering manual review workload for financial institutions

**Personal Contribution**:
- Solely responsible for all model-related work: algorithm selection, code implementation, 5-fold cross-validation, hyperparameter tuning, and model training
- Wrote the complete "Method" of the final group report and created the corresponding presentation slides
- Coordinated with data preprocessing and validation teams to ensure seamless data and model handoff

**Project Link**:
- Group GitHub Repository: [https://github.com/justusyyr/Group-Assignment---Lays](sslocal://flow/file_open?url=https%3A%2F%2Fgithub.com%2Fjustusyyr%2FGroup-Assignment---Lays&flow_extra=eyJsaW5rX3R5cGUiOiJjb2RlX2ludGVycHJldGVyIn0=)

---

### Project 3: Financial Analysis and Monthly Profit Forecast for Entrepreneurial Venture
**Team Project** | 2024.10 - 2024.12

**Problem**: Startups lack accurate financial forecasting tools, making it difficult to assess project feasibility and develop reasonable business plans. This project aims to provide comprehensive financial analysis and reliable monthly profit forecasts for an entrepreneurial venture to support decision-making for investors and management.

**Data**: Built a multi-dimensional financial dataset including revenue, cost, and expenses based on industry benchmark data and market research data.

**Approach**: Adopted financial statement analysis methods and time series forecasting models to conduct cash flow forecasting, break-even analysis, and sensitivity analysis. Integrated financial forecasting results with the overall business plan to ensure reasonableness and feasibility.

**Outcome & Impact**:
- Completed a comprehensive financial feasibility analysis report, identifying key risk points and profit opportunities of the project
- Provided detailed monthly profit forecasts and cash flow forecasts for the next 12 months
- Presented results to investors and management, receiving positive feedback and strong support for project financing

**Personal Contribution**: Led the financial analysis module and monthly profit forecasting model development, wrote the financial section of the report, and delivered the final presentation
