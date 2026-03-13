# Social Media Advertisement Audience Segmentation using Machine Learning

## Project Overview

This project applies **unsupervised machine learning techniques** to analyze social media advertisement interaction data and discover patterns in user engagement behavior.

Using a dataset containing **100,000 advertisement interaction records**, the project identifies natural user segments based on engagement characteristics such as impressions, clicks, conversions, and interaction duration.

Understanding these audience segments can help marketing teams improve **advertisement targeting, user engagement strategies, and campaign performance**.

---

## Dataset

The dataset used in this project is publicly available on Kaggle.

Dataset Link:  
https://www.kaggle.com/datasets/ziya07/social-media-ad-engagement-dataset

The dataset contains **100,000 records** and **35 features**, including:

- User demographics (age, gender, location)
- Device information
- Advertisement category
- User interaction metrics
- Sentiment scores
- Text-based TF-IDF features

---

## Objectives

The main objectives of this project are:

- Discover natural **user engagement patterns** in advertisement interaction data
- Segment users into **distinct behavioral groups**
- Compare the performance of different clustering algorithms
- Visualize cluster structures using dimensionality reduction techniques

---

## Machine Learning Methods Used

### 1. K-Means Clustering
K-Means clustering was used to partition users into distinct groups based on engagement behavior.

Key steps included:
- Data preprocessing
- Feature scaling using **StandardScaler**
- Determining optimal cluster number using the **Elbow Method**
- Cluster visualization using **Principal Component Analysis (PCA)**

### 2. Hierarchical Agglomerative Clustering
Hierarchical clustering was applied to analyze the **hierarchical relationships between clusters**.

A **dendrogram** was generated to visualize how clusters merge based on similarity.

---

## Data Preprocessing

Several preprocessing steps were performed before clustering:

- Removal of identifier columns (`user_id`, `ad_id`, timestamps)
- Feature selection focusing on engagement metrics
- Standardization of numerical features using **StandardScaler**
- Sampling of the dataset for hierarchical clustering to reduce computational cost

---

## Key Visualizations

### Elbow Method

Used to determine the optimal number of clusters for K-Means.

The inertia curve suggested **k = 4** as the optimal cluster count.

---

### PCA Cluster Visualization

Principal Component Analysis (PCA) was used to reduce high-dimensional data into two components for visualization.

Each color represents a different cluster discovered by the K-Means algorithm.

---

### Hierarchical Clustering Dendrogram

A dendrogram was generated to visualize hierarchical cluster relationships and compare clustering structure with K-Means.

---

## Results

The clustering analysis identified **four distinct user segments**:

1. **Low Engagement Users**  
   Users with minimal interaction with advertisements.

2. **Moderate Interaction Users**  
   Users showing occasional advertisement interaction.

3. **Highly Engaged Users**  
   Users frequently clicking and interacting with advertisements.

4. **Heavy Interaction Users**  
   Users with the highest advertisement exposure and engagement levels.

These segments provide insights into **different audience behaviors**, which can help optimize advertising strategies.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- PCA (Principal Component Analysis)

---

## Repository Structure

Social-Media-Ad-Segmentation/
│
├── notebook.ipynb # Main analysis notebook
├── README.md # Project documentation
├── figures/
│ ├── elbow_plot.png
│ ├── pca_clusters.png
│ └── dendrogram.png
└── dataset_link.txt

---

## How to Run the Project

1. Clone the repository - git clone https://github.com/your-username/.git
2. Install required libraries
3. Run the Jupyter notebook


---

## Future Improvements

Possible future improvements include:

- Applying **Dimensionality Reduction techniques** such as t-SNE or UMAP
- Evaluating cluster quality using **Silhouette Score**
- Building a **dashboard for cluster exploration**
- Testing additional clustering algorithms such as DBSCAN

---

## Author

Lakitha Viraj  
Computer Engineering Undergraduate  
University of Ruhuna

---

## License

This project is for educational and research purposes.
