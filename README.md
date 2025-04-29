# 📱 Mobile Phone Price Range Prediction

This project focuses on predicting the price range of mobile phones using various features like hardware specifications and performance metrics. By analyzing a real-world dataset, we aim to develop a predictive model to classify phones into distinct price segments, enabling better market targeting and consumer insight.

---

## 📊 Dataset Overview

The dataset includes **2,000 mobile phones** with **21 features**, such as:

- **Battery Power**
- **RAM**
- **Internal Storage**
- **Camera Specs (Primary, Front)**
- **Display & Resolution**
- **Connectivity (3G, 4G, WiFi, Bluetooth)**
- **Processor Speed**
- **Device Dimensions and Weight**

The **target variable** is the `price_range`:

- `0`: Low Cost  
- `1`: Medium Cost  
- `2`: High Cost  
- `3`: Very High Cost

---

## 🧹 Data Preprocessing

- ✅ No missing values were found.  
- 🔄 All categorical values were already encoded.  
- 🔍 Feature scaling applied where needed.  
- ⚖️ Dataset is balanced across all four price categories.  

---

## 🔍 Exploratory Data Analysis

Key insights:

- 📶 **RAM** and **Battery Power** are strong indicators of price range.  
- 📸 Phones with **dual cameras** (higher `px_height` and `px_width`) tend to fall in higher price segments.  
- 📈 Features like **Processor Frequency**, **Storage**, and **Touchscreen** also influence pricing.  
- ❌ Features like **Bluetooth** and **3G** showed minimal impact on price range prediction.  

---

## 🤖 Machine Learning Task: Multi-Class Classification

We implemented multiple classification algorithms to predict the mobile phone price range. The best results were achieved with the **Random Forest Classifier**.

### 🔝 Best Model: Random Forest

| Metric        | Score |
|---------------|-------|
| Accuracy      | 0.89  |
| F1-Score      | 0.89 (Weighted Avg) |

### 📌 Classification Report:

| Price Range   | Precision | Recall | F1-score |
|---------------|-----------|--------|----------|
| Low (0)       | 0.91      | 0.92   | 0.91     |
| Medium (1)    | 0.87      | 0.84   | 0.85     |
| High (2)      | 0.85      | 0.86   | 0.85     |
| Very High (3) | 0.93      | 0.93   | 0.93     |

---

## ⚙️ Model Comparison

- **Logistic Regression**: Accuracy ~0.65  
- **SVM (RBF Kernel)**: Accuracy ~0.84  
- **K-Nearest Neighbors**: Accuracy ~0.82  
- **Random Forest**: ✅ Best performance at 0.89  

---

## 💡 Insights & Recommendations

- 🔍 **RAM** is the most decisive factor in determining mobile phone prices — optimizing it can provide significant value to consumers.  
- 🎯 Manufacturers can use such predictive modeling for **market segmentation** and **product positioning**.  
- 📉 Features like Bluetooth or 3G can be deprioritized in newer models as they have little impact on price perception.  
- 🚀 *Future Work*: Integrate clustering to define market personas and optimize offerings per segment.

---
