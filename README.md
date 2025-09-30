Socio-Economic Cluster Analysis for NGOs: A Data-Driven Approach to Aid Allocation
📖 Overview
This project uses unsupervised machine learning to help an international humanitarian NGO strategically allocate a $10 million fund. By analyzing socio-economic and health data for 167 countries, we identify and prioritize nations that are in the most dire need of aid. The core of this analysis is the K-means clustering algorithm, which groups countries into distinct categories based on their development status.

🎯 Problem Statement
An international NGO has raised approximately $10 million for humanitarian aid. The CEO needs to decide which countries to focus these funds on to maximize their impact. The challenge is to move beyond anecdotal evidence and use a data-driven approach to identify the countries facing the most severe socio-economic and health crises.

Our task is to classify countries based on key development factors and provide a clear, defensible recommendation for which nations should be the highest priority for this aid program.

🛠️ Methodology
The project follows a standard data science workflow:

Data Preprocessing: The initial dataset (Country-data.csv) was loaded, and all numerical features were scaled using StandardScaler. Scaling ensures that variables with larger ranges (like income) do not disproportionately influence the clustering algorithm.

Optimal Cluster Selection (Elbow Method): To determine the ideal number of country groups, the Elbow Method was used. We calculated the inertia for K values from 1 to 10. The plot showed a distinct "elbow" at K=3, indicating that three clusters is the optimal number for this dataset.

K-means Clustering: With K=3, the K-means algorithm was applied to the scaled data. Each country was assigned to one of three clusters based on its proximity to the cluster's centroid.

Visualization (PCA): To visualize the clusters in two dimensions, Principal Component Analysis (PCA) was used to reduce the dimensionality of the data. This allows us to plot and visually inspect the distinct country groupings.

📊 Results & Analysis
The analysis successfully segmented the countries into three distinct clusters, which can be interpreted as:

Cluster 0: Underdeveloped Countries (Most in need)

Cluster 1: Developing Countries

Cluster 2: Developed Countries

Elbow Method Plot
The plot below clearly shows the "elbow" at K=3, validating our choice of three clusters.

Country Cluster Visualization
The PCA plot visualizes the three clusters, demonstrating a clear separation between the groups based on their overall development indicators.

🏆 Conclusion & Recommendation
Based on the analysis, the countries in Cluster 0 are unequivocally the most in need of humanitarian aid.

It is strongly recommended that the CEO and the NGO board prioritize the 47 countries in this cluster for the $10 million aid program. This data-driven approach ensures that the funds are directed to where they can have the most significant and life-saving impact.
