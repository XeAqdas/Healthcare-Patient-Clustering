# 🧩 Healthcare Patient Segmentation using K-Means Clustering

## 📌 Project Overview
This project applies unsupervised machine learning to segment patients into distinct risk profiles. By clustering medical insurance data, businesses can identify high-cost patient groups and tailor their healthcare strategies or premium pricing accordingly.

## 🛠️ Tech Stack
* **Language:** Python
* **Libraries:** Scikit-Learn (K-Means, StandardScaler, Silhouette Score), Pandas, Seaborn, Matplotlib
* **Environment:** Google Colab

## ⚙️ Model Development
1. **Data Preprocessing:** Standardized numerical features (`age`, `bmi`, `charges`) using `StandardScaler` to ensure unbiased clustering.
2. **Optimal Cluster Selection:** Utilized the **Elbow Method** to determine the optimal number of clusters (k=3).
3. **Model Training:** Applied K-Means clustering in a 3-dimensional feature space.
4. **Validation:** Calculated the **Silhouette Score** to mathematically verify the separation and density of the clusters.

## 📊 Key Business Insights
The K-Means model identified three distinct patient segments:
* **Cluster 0 (Low Risk):** Patients with average BMI and age, driving the lowest medical charges.
* **Cluster 1 (Moderate Risk):** Older patients or those with specific health factors leading to medium medical costs.
* **Cluster 2 (High Risk / High Cost):** A distinct group (heavily correlated with smokers and high BMI) driving extreme medical charges, averaging nearly $40,000. 

## 📂 How to Run
1. Clone this repository.
2. Ensure `insurance.csv` is in the same directory as the notebook.
3. Run the Jupyter Notebook to view the code, 3D pairplots, and distribution boxplots.
