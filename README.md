# Customer Segmentation Using K-Means Clustering (Mall Dataset)

This project applies K-Means clustering to segment customers based on their **Annual Income** and **Spending Score** from the Mall Customers dataset. The segmentation helps businesses understand distinct customer groups and tailor marketing strategies accordingly.

## Overview

Customer segmentation is a powerful marketing tool that allows businesses to understand their customers better by grouping them based on similar characteristics. In this notebook, we:

- Load and preprocess mall customer data
- Encode categorical variables
- Apply K-Means clustering algorithm
- Use the elbow method to determine optimal number of clusters
- Visualize the clusters with Matplotlib

##  Dataset

- **File:** `Mall_Customers.csv`
- **Features:**
  - `CustomerID`: Unique identifier
  - `Genre`: Gender of the customer
  - `Age`: Age of the customer
  - `Annual_Income_(k$)`: Annual income in $1000s
  - `Spending_Score`: Score assigned based on customer behavior and spending nature

##  Libraries Used

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

##  Data Preprocessing

- Encoded the `Genre` column using `LabelEncoder`.
- No missing values found in the dataset.

```python
from sklearn.preprocessing import LabelEncoder
le = LabelEncoder()
data['Genre'] = le.fit_transform(data['Genre'])
