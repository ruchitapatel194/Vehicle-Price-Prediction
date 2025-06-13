# Car Selling Price Analysis

In the competitive landscape of automobile sales, determining a car's selling price involves various factors like brand perception, vehicle condition, and market trends. This project utilizes a dataset of 118,412 car sale records to uncover patterns influencing car prices using data mining techniques. The goal is to provide actionable insights for the automotive industry, guiding pricing strategies and improving understanding of consumer preferences.

**Key Objectives:**

   - Analyze the 'data3.csv' dataset to identify significant factors affecting car prices.
   - Explore relationships between attributes like year, make, model, and condition to understand their influence on pricing.
   - Visualize key trends and insights to make data-driven conclusions.

**Methodology:**

   - **Data Cleaning:** Handled missing values, removed irrelevant columns (e.g., sale date), and used the Interquartile Range (IQR) method for outlier detection.
   - **Data Preparation:** Scaled numerical features and encoded categorical variables for analysis.
   - **EDA & Visualization:** Generated scatter plots, box plots, and pie charts to visualize trends in car conditions, mileage, make, color, and transmission types.
   - **Tools:** Python, Pandas, Seaborn, Matplotlib, and Scikit-learn for data handling, visualization, and statistical analysis.

**Key Findings:**

   - Vehicle condition, make, model, year, and odometer readings strongly correlate with selling prices.
   - Outliers in 'selling price' data indicate rare or luxury vehicles, which could skew average pricing trends.
   - The preference for automatic transmission and specific colors and makes significantly impact car sales.

**Algorithms Used:**

   1. **K-Means Clustering:** Used to segment cars into different price clusters based on year and selling price, allowing for better understanding of market segmentation.

   2. **Hierarchical Clustering:** Applied to identify hierarchical relationships between cars based on year and price, visualized using a dendrogram.

   3. **K-Nearest Neighbors (KNN):** Implemented to classify cars into price categories (above or below $11,000) using features like year, odometer reading, and condition. The model achieved strong accuracy, validated by the classification report and confusion matrix.

   4. **Linear Regression:** Used to predict car selling prices based on features such as year, odometer reading, and condition. The model provided strong performance with low Root Mean Squared Error (RMSE) and Mean Absolute Error (MAE).

**Exploratory Data Analysis (EDA) and Visualizations:**

The visualizations generated from the dataset highlighted several important trends:

   **Boxplot Analysis:** A positive skew in the distribution of 'sellingprice' was observed, with outliers indicating the sale of luxury or rare vehicles, which significantly affect the average pricing.
   
   **Scatter Plots:** Clusters emerged when plotting 'sellingprice' against 'odometer' readings and 'condition', illustrating the depreciation of vehicle value as mileage increases and condition worsens.
   
   **Pie Charts:** A clear preference for automatic transmissions was evident in the dataset, indicating a dominant trend among the vehicles sold.
   
   **Bar Charts:** Certain car makes and colors were favored, suggesting these factors may influence selling prices and consumer demand.
   
   **Line Charts:** A noticeable upward trend in selling prices over the years could be attributed to inflation or shifts in consumer preferences toward higher-priced models.

   ![photo_2024-09-13_18-27-09](https://github.com/user-attachments/assets/07593649-a3ac-4df9-a1d9-eb8cf9c01391)

**Results:**

   - The KNN classifier accurately predicted price categories, confirmed by a high classification report score and a well-formed confusion matrix.

      ![image](https://github.com/user-attachments/assets/9ecc9c3b-dfe6-4c17-8de1-5365e5fa27de)

   - The Linear Regression model achieved an RMSE of 5267.36 and an MAE of 4070.18, demonstrating its effectiveness in estimating car selling prices with room for improvement.

      ![image](https://github.com/user-attachments/assets/c8d18a04-2a35-44b2-a45a-687a4f9d1d68)

   - Cluster analysis using K-Means and Hierarchical Clustering revealed clear segmentation of car prices based on features such as the year of the car and its condition.

      ![image](https://github.com/user-attachments/assets/31987652-10e0-4d40-b1f8-4a47f6275fe4)

      ![image](https://github.com/user-attachments/assets/093f4a4b-164d-482b-81b1-50bdaaf76310)

      ![image](https://github.com/user-attachments/assets/0ca76e1b-2161-4655-aab5-82e5f2b07af9)



