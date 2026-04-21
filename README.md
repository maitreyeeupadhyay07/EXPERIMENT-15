
# **Experiment 15: Data Normalization and Data Type Conversion**

## **Aim**

To study and implement different data normalization techniques and convert categorical data into numerical form using Python libraries such as Pandas and NumPy.

---

## **Theory**

### **1. Data Normalization**

Data normalization is a preprocessing technique used to scale numerical data into a specific range or distribution. It is essential because datasets often contain features with different units and magnitudes, which can negatively affect machine learning models and data analysis.

Normalization ensures that all features contribute equally to the analysis.

### **Types of Normalization Used:**

#### **a) Min-Max Normalization**

This method scales data into a fixed range, usually **0 to 1**.

Formula:
[
X' = \frac{X - X_{min}}{X_{max} - X_{min}}
]

* Preserves relationships between values
* Sensitive to outliers
* Used in your experiment for **price and multiple columns**

---

#### **b) Z-Score Normalization (Standardization)**

This method transforms data so that it has a **mean of 0** and **standard deviation of 1**.

Formula:
[
Z = \frac{X - \mu}{\sigma}
]

* Useful when data follows a normal distribution
* Less affected by outliers
* Applied to **units_sold** in your experiment

---

#### **c) Decimal Scaling**

In this method, values are scaled by moving the decimal point.

Formula:
[
X' = \frac{X}{10^j}
]

Where *j* is chosen such that the maximum absolute value is less than 1.

* Simple method
* Used for **price scaling** in your experiment

---

### **2. Data Type Conversion (Categorical to Numerical)**

Real-world datasets often contain categorical variables (text data), which must be converted into numerical form for analysis.

#### **a) Label Encoding**

* Assigns a unique integer to each category
* Example: Male = 0, Female = 1
* Suitable for ordinal data
* Used for **Customer Gender and City**

**Limitation:** May introduce unintended order

---

#### **b) One-Hot Encoding**

* Creates separate binary columns for each category
* Example: Payment_Method → UPI, COD, etc. become columns
* No ordinal relationship introduced

**Advantages:**

* More accurate for nominal data
* Widely used in machine learning

**Disadvantages:**

* Increases dimensionality

---

### **Importance of These Techniques**

* Improves model accuracy
* Prevents bias due to scale differences
* Makes data suitable for algorithms
* Essential step in data preprocessing

---

## **Conclusion**

In this experiment, various normalization techniques such as **Min-Max scaling, Z-score normalization, and Decimal scaling** were successfully applied to numerical data. Additionally, categorical data was converted into numerical form using **Label Encoding and One-Hot Encoding**.

These techniques are crucial in data preprocessing as they improve data quality, ensure uniformity, and make datasets suitable for analysis and machine learning models.

---
