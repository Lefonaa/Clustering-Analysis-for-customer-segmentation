# Customer Segmentation Analysis 📊

## Project Overview
This project develops a clustering solution for an online retailer to segment customers based on demographic and behavioral attributes. By grouping customers using **Annual Income** and **Spending Score**, the business can move from broad marketing to highly personalized, data-driven strategies.

## Author
* **Lefona Moloi**
* **Education**: 3rd Year BSc in Information Technology (Data Science), Eduvos

## Dataset
The analysis uses the `customer_segmentation.csv` dataset, which contains records for over 1,000 customers.
* **Feature Selection**: Focused on `income` and `spending_score` to identify core purchasing patterns.
* **Preprocessing**: Handled missing values and dropped irrelevant columns to improve model accuracy.

## Technical Workflow
1. **Exploratory Data Analysis**: Visualized initial data distribution via scatter plots.
2. **Optimal Cluster Selection**: Utilized the **Elbow Method** to calculate the Within-Cluster Sum of Squares (WCSS).
3. **Model Training**: Applied the **KMeans** algorithm from `sklearn.cluster` using the identified optimal cluster count.
4. **Visualization**: Plotted the final segments with distinct colors and identified the **centroids** for each group.

## Visualizations
### Elbow Method for Optimal K
![Elbow Graph](visualisations/Elbow%20Graph.png)

### Final Customer Segments
![Customer Groups](visualisations/customer%20groups.png)

## Results & Interpretation
The analysis successfully formed **5 distinct customer clusters**:
* **Cluster 1**: High Income, Low Spending Score (Frugal/Careful Spenders).
* **Cluster 2**: High Income, High Spending Score (Target Customers/VIPS).
* **Cluster 3**: Average Income, Average Spending Score (Standard Customers).
* **Cluster 4**: Low Income, High Spending Score (Impulsive Spenders).
* **Cluster 5**: Low Income, Low Spending Score (Sensible/Budget Spenders).

### Business Impact
This clustering output assists the retailer in tailoring advertisements by:
* **Targeting High-Value Segments**: Directing premium loyalty offers to high-income/high-spend groups.
* **Re-engagement**: Sending specialized discount vouchers to high-income/low-spend customers.
* **Budget Optimization**: Focusing essential, low-cost product ads toward the lower-income segments.

## Technologies Used
* **Python** (Pandas, Matplotlib, Seaborn, Scikit-Learn)

## How to Use
1. Clone the repository.
2. Ensure `customer_segmentation.csv` is in the root directory.
3. Run the Jupyter Notebook to generate the plots and analysis.
