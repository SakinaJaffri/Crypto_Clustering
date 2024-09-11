# Crypto Clustering (Unsupervised Learning)

![Crypto Image](https://github.com/SakinaJaffri/Crypto_Clustering/assets/146900226/57c597d0-ac2b-4352-bd90-5e38710cc00f)

## Overview

This project applies **unsupervised learning** techniques, particularly **K-means clustering**, to analyze cryptocurrency data. Using Python, the goal is to explore patterns in price changes over 24 hours and 7 days for various cryptocurrencies, and predict their behavior based on clustering.

## Project Workflow

### 1. Data Preparation
- Normalized the cryptocurrency data using `StandardScaler()` from `scikit-learn`.
- Created a DataFrame with the scaled data, setting `"coin_id"` as the index.

### 2. Finding the Optimal k Value
- Applied the **elbow method** to identify the best value of k (number of clusters).
- Tested k values from 1 to 11 and calculated inertia for each.
- Plotted a line chart to visualize inertia and select the optimal k value.

### 3. Clustering Cryptocurrencies with K-means
- Used the best k value obtained from the elbow method to cluster the original scaled data.
- Generated a **scatter plot** displaying clusters based on 24-hour and 7-day price changes.

### 4. Principal Component Analysis (PCA)
- Performed **PCA** to reduce the dataset to three principal components for simplified clustering.
- Analyzed the explained variance for each component to evaluate their contribution.

### 5. Finding the Best k Value for PCA Data
- Applied the elbow method again on the PCA-transformed data to find the best k value for clustering.

### 6. Clustering Cryptocurrencies with K-means (PCA Data)
- Clustered cryptocurrencies using the optimal k value determined from the PCA data.
- Visualized the clusters using a scatter plot based on the PCA components.

## Results
The project successfully clustered cryptocurrencies based on their price change patterns over short-term periods (24 hours and 7 days), both with the original scaled data and after applying PCA for feature reduction. These clusters help reveal trends in cryptocurrency market behavior.

## Technologies Used
- **Python**
- **Pandas**
- **Scikit-learn**
- **Matplotlib**
- **K-means Clustering**
- **Principal Component Analysis (PCA)**

## How to Use
1. Clone the repository to your local machine.
2. Install the required dependencies listed in `requirements.txt`.
3. Run the Jupyter Notebook provided to execute the analysis and visualize the clusters.

## Conclusion
This project showcases the use of unsupervised learning techniques for analyzing cryptocurrency data. It highlights the importance of feature scaling and dimensionality reduction for efficient clustering, and demonstrates how machine learning models can be used to identify trends in complex datasets.

## Contributors
- **Sakina Jaffri** - Project Developer
