# Crypto_Clustering


**Introduction:**

In this project, I utilized Python and unsupervised learning techniques to analyze cryptocurrency data. The goal was to predict the impact of price changes over 24 hours or 7 days on various cryptocurrencies.

**Data Preparation:**

- Normalized the data using the StandardScaler() module from scikit-learn.
- Created a DataFrame with the scaled data, setting "coin_id" as the index.

**Finding the Best k Value with Original Scaled Data:**

- Applied the elbow method to determine the optimal k value.
- Tested k values ranging from 1 to 11 and computed inertia values for each.
- Plotted a line chart to visualize inertia and identify the best k.

**Clustering Cryptocurrencies with K-means (Original Scaled Data):**

- Clustered cryptocurrencies using the best k value obtained.
- Generated a scatter plot with price change percentages for 24 hours and 7 days.

**Optimizing Clusters with Principal Component Analysis (PCA):**

- Conducted PCA to reduce features to three principal components.
- Evaluated explained variance to understand each component's contribution.

**Finding the Best k Value with PCA Data:**

- Utilized the elbow method on PCA data to find the best k value.

**Clustering Cryptocurrencies with K-means (PCA Data):**

- Clustered cryptocurrencies using the best k value determined from PCA.
- Plotted a scatter plot with PCA components.

This project facilitated the identification of patterns in cryptocurrency data and clustering based on price change trends.
