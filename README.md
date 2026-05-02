# Machine Learning Mini-Projects: Regression & Clustering

This repository contains two machine learning projects implemented in Python using Jupyter Notebooks. The projects cover supervised learning (Multiple Linear Regression) and unsupervised learning (K-Means Clustering). 

## 1. Multiple Linear Regression: Startup Profit Prediction

This project predicts the profit of a startup based on its expenditures and location[cite: 1]. 

### Dataset
*   **File**: `50_Startups.csv`[cite: 1]
*   **Features**: R&D Spend, Administration, Marketing Spend, and State[cite: 1].
*   **Target**: Profit[cite: 1].

### Key Steps
*   **Data Preprocessing**: The categorical 'State' column is encoded using `OneHotEncoder` and `ColumnTransformer`[cite: 1]. 
*   **Dataset Splitting**: The data is split into a Training set (80%) and a Test set (20%)[cite: 1].
*   **Model Training**: A `LinearRegression` model from `scikit-learn` is trained on the dataset[cite: 1].
*   **Prediction**: The model predicts the profits for the test set, and can also be used to predict the profit of a single custom observation (e.g., a startup in State 1 with 160k R&D, 130k Admin, and 300k Marketing spend)[cite: 1].

---

## 2. K-Means Clustering: Mall Customer Segmentation

This project groups mall customers into different segments based on their annual income and spending habits[cite: 2].

### Dataset
*   **File**: `Mall_Customers.csv`[cite: 2]
*   **Features Used**: Annual Income (k$) and Spending Score (1-100)[cite: 2].

### Key Steps
*   **The Elbow Method**: The model iterates through 1 to 10 clusters to calculate the Within-Cluster Sum of Squares (WCSS) and plots an Elbow graph to determine the optimal number of clusters[cite: 2].
*   **Model Training**: Based on the Elbow method, a `KMeans` model is trained to create exactly 5 clusters[cite: 2].
*   **Visualization**: The results are plotted using `matplotlib` on a 2D scatter plot, distinctly showing the 5 customer segments (colored red, blue, green, cyan, and magenta) alongside their respective yellow centroids[cite: 2].

---

## Dependencies

To run these notebooks, you will need the following Python libraries installed[cite: 1, 2]:
*   `numpy`
*   `pandas`
*   `matplotlib`
*   `scikit-learn`

## How to Run
1. Clone this repository.
2. Ensure you have Jupyter Notebook or JupyterLab installed, or upload the notebooks to Google Colab.
3. Make sure the dataset files (`50_Startups.csv` and `Mall_Customers.csv`) are in the same directory as the notebooks.
4. Run the cells sequentially.
