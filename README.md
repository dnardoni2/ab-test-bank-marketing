# ab-test-bank-marketing
A/B test using the UCI Bank Marketing dataset to evaluate campaign strategies and improve conversion.

# A/B Test — Bank Marketing Campaign Optimization  
Using the UCI Bank Marketing Dataset

## 📌 Project Overview
This project simulates an A/B test to evaluate marketing strategies used by a financial institution to promotw term deposit subscriptions

  **Version A (Control):** Standard, non-personalized campaign strategy.  
  **Version B (Treatment):** Segmented campaign tailored by customer profile (job, age group, education, marital status).
  
The goal is to determine whether segmentation leads to a statistically significant improvement in the conversion rate.

## 📁 Dataset
This project uses the **Bank Marketing dataset**, provided by the University of California Irvine (UCI Machine Learning Repository).

Dataset link:  
https://archive.ics.uci.edu/ml/datasets/Bank+Marketing

**Observations:**  
- 45,211 marketing contacts  
- Features describing customer profile and campaign interactions  
- Target variable: `y` (yes/no for term deposit subscription)

---

## 🎯 Business Question & Hypotheses

### **Business Question**
Can a segmented marketing strategy increase the conversion rate of term deposit subscriptions compared to a standard strategy?

### **Hypotheses**

**H₀ — Null Hypothesis:**  
There is *no significant difference* in conversion rates between the standard campaign (A) and the segmented campaign (B).

**H₁ — Alternative Hypothesis:**  
The segmented campaign (B) leads to a *higher conversion rate* than the standard campaign (A).

---

## 🧪 Experiment Design

### **Group A — Control**
Simulated sample using the original dataset distribution (baseline).

### **Group B — Treatment**
Simulated sample applying segmentation rules:
- Younger customers receive shorter, objective messages  
- Older customers receive more detailed messages  
- Customers with higher education or stable jobs receive personalized financial benefits  
- Retired customers receive safer, low-risk messaging  

### **Primary Metric**
- **Conversion Rate**  
  `conversion = subscribed / total_customers`

### **Secondary Metrics**
- Conversion by age group  
- Conversion by job type  
- Conversion by marital status  
- Conversion by education level  

### **Statistical Test**
- Two-Proportion Z-Test  
- 95% confidence level  
- Effect size evaluation  
- Confidence intervals for both groups
