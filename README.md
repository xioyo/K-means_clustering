# K-Means Clustering

## Objective  
To apply **K-Means clustering** on the Mall Customers dataset to identify customer segments and visualize them using PCA. The goal is to understand customer groupings based on demographic and spending behavior.

---

## Dataset  
- **Source:** Mall Customers dataset  
- **Features:** CustomerID, Gender, Age, Annual Income (k$), Spending Score (1–100)  
- **Target:** No target column (unsupervised learning)  

---

## Workflow  
1. **Load & Explore Data**  
   - Imported dataset using Pandas and explored features.  

2. **Preprocessing**  
   - Converted categorical features (Gender) into numeric format.  
   - Scaled all features using `StandardScaler` for uniformity.  

3. **Finding Optimal K (Elbow Method)**  
   - Ran K-Means for K values from 1 to 10.  
   - Chose **K = 5** based on the elbow point in the inertia curve.  

4. **K-Means Clustering**  
   - Trained K-Means model with 5 clusters.  
   - Assigned cluster labels to each customer.  

5. **Evaluation**  
   - **Silhouette Score:** 0.554 (indicates moderate clustering quality).  

6. **Visualization**  
   - Applied **PCA (2 components)** for dimensionality reduction.  
   - Plotted customers in 2D space with color-coded clusters.  

---

## Results & Inference  
- Customers are clearly grouped into **5 clusters** based on income, spending, and demographics.  
- Some clusters are well-separated (distinct spending behaviors), while others have slight overlaps.  
- Businesses can target marketing strategies differently for each group.

---

## Technologies Used  
- Python  
- Pandas, NumPy  
- Scikit-learn (`KMeans`, `StandardScaler`, `PCA`)  
- Matplotlib, Seaborn  