# Advanced-Customer-Segmentation-Using-Apache-Spark-K-Means-vs.-GMM-in-Retail-Analytics
 Scalable Systems Programming
Here’s a draft for the README file based on the content of the provided files:

---

# Advanced Customer Segmentation Using Apache Spark

## Overview
This project demonstrates customer segmentation techniques for retail analytics using clustering algorithms, implemented in PySpark on Databricks. Two clustering methods, K-Means and Gaussian Mixture Model (GMM), are compared based on their efficiency and accuracy.

---

## Project Structure
1. Streamlined_Data.ipynb  
   Handles data preprocessing, including cleaning, transformation, and feature engineering.

2. KMeans_Algorithm-001.ipynb  
   Implements the K-Means clustering algorithm with evaluation metrics such as:
   - Elbow Method
   - Silhouette Score
   - Davies-Bouldin Index

3. GaussianMM_Algorithm-002.ipynb  
   Implements the Gaussian Mixture Model clustering algorithm, evaluating the results using:
   - Silhouette Score
   - Davies-Bouldin Index

4. Environment Setup and Workflow  
   Provides detailed instructions for setting up the environment and workflow in Databricks.

---

## Environment Setup
1. Cluster Configuration:
   - Worker Type: i3.xlarge (30.5 GB Memory, 4 Cores)
   - Min Workers: 6
   - Max Workers: 8
   - Driver Type: i3.xlarge
   - Runtime Version: 14.3 LTS (Apache Spark 3.5.0, Scala 2.12)
   - Photon Acceleration: Enabled
   - Autoscaling: Enabled

2. Data Upload:  
   The dataset (`Mall_Customers.csv`) is uploaded via the Databricks File System (DBFS).

3. Tools and Libraries:
   - PySpark
   - StandardScaler
   - PCA
   - StringIndexer
   - OneHotEncoder
   - VectorAssembler

---

## Methodology
### Data Preprocessing
- StringIndexer: Converts categorical variables to numeric.
- OneHotEncoder: Encodes categorical variables as binary vectors.
- VectorAssembler: Combines multiple features into a single feature vector.
- StandardScaler: Scales features to unit variance.
- PCA: Reduces dimensionality for computational efficiency.

### Clustering Techniques
1. K-Means Clustering:
   - Partition-based clustering.
   - Optimal clusters determined using the Elbow Method.
   - Evaluated using Silhouette Score and Davies-Bouldin Index.

2. Gaussian Mixture Model (GMM):
   - Density-based clustering with probabilistic modeling.
   - Evaluated using Silhouette Score and Davies-Bouldin Index.

---

## Results
- The clustering results are evaluated for quality and efficiency using various metrics.
- Comparative insights between K-Means and GMM are highlighted.

---

## MapReduce Framework in PySpark
PySpark's RDD and DataFrame APIs are leveraged for distributed processing:
- Map Operations: Feature transformation and scaling.
- Reduce Operations: Clustering and aggregation of results.

---

## How to Run the Project
1. Upload the dataset to DBFS.
2. Set up the Databricks cluster using the specified configuration.
3. Execute the notebooks in the following order:
   - Streamlined_Data.ipynb
   - KMeans_Algorithm-001.ipynb
   - GaussianMM_Algorithm-002.ipynb
4. Analyze the output metrics and visualizations for clustering quality.

---

## Author
Priyanka Bundela  
