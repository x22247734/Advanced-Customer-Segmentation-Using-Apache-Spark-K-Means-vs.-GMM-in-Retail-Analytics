# Advanced-Customer-Segmentation-Using-Apache-Spark-K-Means-vs-GMM-in-Retail-Analytics

## 📊 Advanced Customer Segmentation Using Apache Spark

### 🚀 Overview  
This project applies advanced clustering techniques—**K-Means** and **Gaussian Mixture Model (GMM)**—for customer segmentation in the retail domain. Implemented using **PySpark** on **Databricks**, the goal is to compare the performance and clustering quality of both models in a big data environment.

---

### 🗂️ Project Structure

| File/Notebook                    | Description                                                                 |
|----------------------------------|-----------------------------------------------------------------------------|
| `Streamlined_Data.ipynb`         | Data cleaning, transformation, and feature engineering.                    |
| `KMeans_Algorithm-001.ipynb`     | Implements K-Means with Elbow Method, Silhouette Score, and Davies-Bouldin.|
| `GaussianMM_Algorithm-002.ipynb` | Implements GMM with Silhouette Score and Davies-Bouldin Index.             |
| `README.md`                      | Project documentation and setup instructions.                              |

---

### ⚙️ Environment Setup

**Cluster Configuration (Databricks):**
- **Worker Type:** i3.xlarge (30.5 GB, 4 Cores)
- **Driver Type:** i3.xlarge
- **Min/Max Workers:** 6–8
- **Runtime Version:** 14.3 LTS (Spark 3.5.0, Scala 2.12)
- **Photon Acceleration:** Enabled
- **Autoscaling:** Enabled

**Libraries & Tools:**
- PySpark
- StandardScaler, PCA
- StringIndexer, OneHotEncoder
- VectorAssembler

**Dataset:**
- `Mall_Customers.csv` (uploaded via DBFS)

---

### 🔬 Methodology

#### ✅ Data Preprocessing
- `StringIndexer` – Encodes categorical features.
- `OneHotEncoder` – Converts to binary vectors.
- `VectorAssembler` – Combines features into a vector.
- `StandardScaler` – Normalizes the data.
- `PCA` – Dimensionality reduction to improve clustering efficiency.

#### 📌 Clustering Algorithms

1. **K-Means**
   - Centroid-based clustering.
   - Uses Elbow Method for optimal clusters.
   - Evaluation: Silhouette Score, Davies-Bouldin Index.

2. **Gaussian Mixture Model (GMM)**
   - Probabilistic model-based clustering.
   - Evaluation: Silhouette Score, Davies-Bouldin Index.

---

### 📈 Results

- Detailed comparison of clustering performance (K-Means vs. GMM).
- Visualizations and metrics for interpretability.
- Highlights strengths of each model based on use-case.

---

### 🔁 MapReduce Perspective (PySpark)

This project leverages PySpark's distributed computing paradigm:
- **Map:** Transformations like scaling, encoding, vectorizing.
- **Reduce:** Cluster evaluation and aggregation.

---

### ▶️ How to Run the Project

1. Upload `Mall_Customers.csv` to DBFS.
2. Create the Databricks cluster with the specified configuration.
3. Run notebooks in the following order:
   - `Streamlined_Data.ipynb`
   - `KMeans_Algorithm-001.ipynb`
   - `GaussianMM_Algorithm-002.ipynb`
4. Analyze output visualizations and metric comparisons.

---

### 👩‍💻 Author  
**Priyanka Bundela**
