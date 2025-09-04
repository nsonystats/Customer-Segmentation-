
						 Customer Segmentation & Churn Prediction Using Clustering and Machine Learning

Project Overview:

In today's data-driven economy, understanding customer behavior is vital for business growth, profitability, and long-term retention. This project leverages unsupervised and supervised machine learning techniques to segment customers and predict churn, thereby enabling targeted retention strategies and optimized business decisions.

Using Principal Component Analysis (PCA) for dimensionality reduction, K-Means and Agglomerative Clustering for segmentation, and Logistic Regression for churn prediction, this project provides deep insights into customer behavior and actionable intelligence for proactive engagement.

Objectives: 

Customer Segmentation: Categorize customers into meaningful groups based on their purchasing patterns using K-Means and Hierarchical Clustering.
Churn Prediction: Predict customer churn using Logistic Regression and provide business recommendations based on the churn risk level.
Business Impact: Suggest data-driven, personalized retention strategies to improve loyalty, maximize revenue, and minimize churn.

Techniques & Tools Used:

1. Principal Component Analysis (PCA)
   - Reduced high-dimensional data while retaining 97.4% of total variance (PC1 + PC2).
   - Enabled clear 2D visualization and efficient clustering.

2. K-Means Clustering
   - Optimal number of clusters selected using the Elbow Method (k = 4).
   - Achieved a high Silhouette Score of 0.7753, indicating well-separated clusters.

3. Agglomerative Hierarchical Clustering
   - Built a hierarchical dendrogram using Ward’s linkage method.
   - Captured nested relationships between customers.
   - Moderate Silhouette Score: 0.4899.

4. Logistic Regression
   - Developed churn prediction model with engineered features: Recency, Frequency, and Monetary Value.
   - Achieved AUC = 0.941, indicating excellent predictive performance.


Methodology: 


Data Preprocessing:

* Removed missing values (135080 null entries in CustomerID).
* Engineered key features: `Transaction`, `Recency`, `Monetary`, `Total_Spend`.
* Standardized variables using Z-score normalization.


Dimensionality Reduction:

* Applied PCA to reduce dimensions for clustering.
* Scree plot showed 2 principal components were sufficient.


Clustering:

* K-Means: 4 clusters identified via Elbow Method.
* Agglomerative Clustering: Hierarchical merging with Ward’s method.
* Clusters analyzed based on visual separation, density, and Silhouette Scores.


Churn Prediction: 

* Churn defined as no purchases since 1st September 2011.
* Logistic Regression model with `binomial` family used.
* Key predictors: Recency (positive churn correlation), Transactions (negative loyalty), Monetary (loyalty indicator).



Key Results: 

* PCA captured 97.4% of variance using only 2 components.
* K-Means Silhouette Score: 0.7753 (excellent segmentation).
* Churn Model AUC: 0.941(strong classification ability).
* Customers with high recency and low transaction frequency are most likely to churn.



Business Applications: 

* Proactive Retention: Early churn detection enables targeted offers and support.
* Revenue Optimization: Retaining customers is 5–7x cheaper than acquiring new ones.
* Personalized Marketing: Segment-based targeting boosts campaign ROI.


Tech Stack:

* Language: R
* Libraries: `ggplot2`, `factoextra`, `cluster`, `caret`, `glm`, `pROC`, `dplyr`, `tidyr`, `scales`
* Tools: Excel, Jupyter (R Kernel), Git, GitHub


Author:
Nitika Sony
MSc Applied Statistics | Symbiosis Statistical Institute


