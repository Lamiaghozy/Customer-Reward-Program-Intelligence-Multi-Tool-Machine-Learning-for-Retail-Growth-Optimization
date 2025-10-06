🧠 Multi-Tool Machine Learning for Retail Reward Optimisation 
A KNIME, RapidMiner & Python Comparative Analytics Project

📌 Overview

This project demonstrates end-to-end application of machine learning techniques across three leading analytics platforms — KNIME, RapidMiner, and Python (scikit-learn) — to predict and optimise customer reward programs for retail businesses.

It was designed to compare model performance across tools, strengthen cross-platform BI & ML expertise, and extract actionable insights relevant to real-world retail strategy.

🎯 Business Objective

Retailers often face the challenge of identifying which factors drive customer reward adoption and effectiveness.
This project explores:

Which business metrics best predict reward participation

How tree-based models and neural networks perform in classification and regression tasks

How bagging and boosting affect predictive performance

🧩 Dataset

Name: Retail_RewardProgram.xlsx

Size: 40 records × 8 columns

Source: Provided dataset for academic BI/ML exercises

Key Features

| Feature           | Description                                                 |
| ----------------- | ----------------------------------------------------------- |
| `Salerank`        | Retailer sales ranking                                      |
| `X2013USSales`    | 2013 U.S. sales figures                                     |
| `X2013WorldSales` | 2013 global sales                                           |
| `ProfitMargin`    | Retailer’s profit margin                                    |
| `NumStores`       | Number of retail stores                                     |
| `IndustryType`    | Retail industry classification                              |
| `Reward`          | Binary target (1 = participates in reward program, 0 = not) |
| `RewardSize`      | Continuous target used for neural network regression        |

⚙️ Tools & Technologies

| Platform                      | Purpose                                                    |
| ----------------------------- | ---------------------------------------------------------- |
| **KNIME**                     | Classification Trees, Boosted Trees                        |
| **RapidMiner**                | Bagging & Boosting (Decision Tree, Neural Network)         |
| **Python**                    | scikit-learn implementation for Bagged Trees & Neural Nets |
| **Excel / CSV**               | Data preprocessing                                         |
| **Matplotlib, Pandas, Numpy** | Data handling & visualization                              |

🧪 Experiments & Results

1️⃣ Classification Tree (KNIME)

Target: Reward
Predictors: Salerank, X2013USSales, X2013WorldSales, ProfitMargin, NumStores, IndustryType

✅ Feature with highest importance: ProfitMargin

2️⃣ Bagged Tree (KNIME / RapidMiner / Python)

Split: 60% training / 40% validation
Metric: Precision (Validation set)

📊 Precision: 0.5000
(Model correctly predicted 50% of positive reward cases on unseen data.)

3️⃣ Boosted Tree (KNIME)

Metric: Precision (Validation set)
📊 Precision: 0.5000

4️⃣ Bagged Neural Network (RapidMiner / Python)

Target: RewardSize
Metric: RMSE (Validation set)
📉 RMSE: 9.3525

5️⃣ Boosted Neural Network (RapidMiner / Python)

Target: RewardSize
Metric: RMSE (Validation set)
📉 RMSE: 9.2408

📸 Visuals & Workflows

| Tool       | Screenshot                                                                                | Description                          |
| ---------- | ----------------------------------------------------------------------------------------- | ------------------------------------ |
| KNIME      | ![KNIME Workflow]([notebooks/knime_workflow_screenshots/knime_workflow.png](https://github.com/Lamiaghozy/Customer-Reward-Program-Intelligence-Multi-Tool-Machine-Learning-for-Retail-Growth-Optimization/blob/main/Data/knime_workflow.png?raw=true))                | End-to-end classification tree setup |
| RapidMiner | ![RapidMiner Workflow](notebooks/rapidminer_workflow_screenshots/rapidminer_workflow.png) | Bagged/Boosted NN configuration      |
| Python     | ![Python Results](notebooks/python_results/python_tree_precision_output.png)              | RMSE output              |

💡 Insights

Profit margin is the most influential factor in predicting reward program participation.

Ensemble methods (bagging/boosting) provide moderate improvement in stability but limited uplift on small datasets.

Neural networks show consistent RMSE performance, suggesting diminishing returns with a small sample size.

Demonstrates strong cross-platform mastery—a key advantage for data science roles requiring tool flexibility.
