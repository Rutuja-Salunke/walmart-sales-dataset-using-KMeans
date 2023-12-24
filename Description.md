# Walmart Store Sales Analysis and Customer Segmentation
## Project Goals and Background

In the 21st century, huge amounts of data are generated, especially in technology-driven sectors like retail. Walmart, a major retail player, relies on data to predict future sales and compete globally. With over 11,000 stores worldwide, understanding customer behavior is vital. This research aims to forecast Walmart's sales based on historical data, considering factors like temperature and holidays. By analyzing past data and using big data analytics, Walmart can optimize sales, promotions, and resources, ensuring competitiveness and profitability in the dynamic market.

## Purpose Statement:
This study aims to predict how much Walmart will sell each week based on data collected from 45 different stores across the country, spanning from 2010 to 2013. The dataset includes information about store size, type, departments, weekly sales, and whether it's a holiday week. We're looking at various factors like Consumer Price Index, temperature, fuel prices, promotions, and unemployment rates to figure out if they influence weekly sales. It helps understand the patterns and connections between sales and these factors.
This study also includes an extensive exploratory data analysis on the provided Walmart dataset to understand the following:
• Identifying store as well as department-wide sales in Walmart
• Identifying sales based on store size and type
• Identifying how much sales increase during holidays
• Correlation between the different factors that affect sales
• Average sales per year
• Weekly sales as per region temperature, CPI, fuel price, unemployment

Objective:
The objective of this project is to analyze the sales data from Walmart stores and perform customer segmentation using clustering techniques. The analysis aims to identify patterns in sales data and group stores or customers based on similar characteristics. This segmentation can provide valuable insights for targeted marketing strategies, inventory management, and overall business optimization.

Project Steps:

1. **Data Gathering:**
   - The project starts with the collection of data from Walmart stores. The dataset includes information such as store details, weekly sales, holiday flags, temperature, fuel prices, CPI (Consumer Price Index), and unemployment rates.

2. **Exploratory Data Analysis (EDA):**
   - Conduct an exploratory data analysis to understand the structure and characteristics of the dataset.
   - Check for missing values, data types, and descriptive statistics.
   - Perform feature engineering if needed, such as dropping unnecessary columns.

3. **Outlier Detection and Handling:**
   - Identify and handle outliers in the dataset to ensure that they do not negatively impact the clustering results.
   - Utilize statistical methods to detect and replace outliers.

4. **Data Scaling:**
   - Standardize the numerical features using Standard Scaler to bring them to a common scale.
   - This step ensures that all features contribute equally to the clustering process.

5. **2D Clustering:**
   - Explore 2D clustering using different pairs of features, such as Temperature vs. Fuel Price, Holiday_Flag vs. Fuel_Price, and Temperature vs. CPI.
   - Apply the KMeans clustering algorithm to group data points.
   - ![Screenshot 2023-12-22 162707](https://github.com/Rutuja-Salunke/walmart-sales-dataset-using-KMeans/assets/102023809/d9dac7e7-8311-4181-8d86-3a19fc2e92a3)
   - ### 5.1. Impact of Temperature on Fuel Price:
In the 2D clustering analysis focusing on temperature and fuel price, the objective is to uncover patterns and relationships between these two key factors and their impact on Walmart store sales. By applying the KMeans clustering algorithm to the dataset, we aim to group data points based on similarities in temperature and fuel price. The visual representation of these clusters provides insights into how variations in temperature and fuel prices contribute to distinct sales patterns. This analysis serves as a foundation for understanding the interplay between environmental and economic factors, aiding in targeted decision-making for sales optimization and resource management at Walmart stores.
   - ![2D-2](https://github.com/Rutuja-Salunke/walmart-sales-dataset-using-KMeans/assets/102023809/e0ea0d5b-3c60-4694-af59-a2d360a48608)
   - ### 5.2. 2D Clustering on Holiday_Flag and Fuel_Price:
   - In the 2D clustering analysis focused on 'Holiday_Flag' and 'Fuel_Price,' the goal is to explore how holidays and fuel prices influence Walmart store sales. By employing the KMeans clustering algorithm, the dataset is partitioned into clusters based on similarities in holiday flags and fuel prices. The resulting clusters reveal distinct patterns in sales behavior associated with holidays and fluctuations in fuel prices. This analysis provides valuable insights into the impact of these external factors on consumer spending, aiding Walmart in formulating targeted strategies for promotions, inventory management, and resource allocation during holiday seasons and varying fuel price conditions.
   - ![2D-3](https://github.com/Rutuja-Salunke/walmart-sales-dataset-using-KMeans/assets/102023809/2d1dce90-a10a-4126-8e0b-a35f846ed93c)
   - ### 5.3. 2D Clustering on Temperature and CPI:
In the 2D clustering analysis centered around 'Temperature' and 'Consumer Price Index (CPI),' the objective is to examine the relationship between weather conditions and economic indicators on Walmart store sales. Utilizing the KMeans clustering algorithm, the dataset is segmented into clusters based on similarities in temperature and CPI. The resulting clusters offer insights into the combined effects of temperature variations and economic trends on consumer behavior and purchasing patterns. This analysis helps Walmart understand the nuanced interactions between weather and economic factors, facilitating informed decision-making for sales strategies, inventory management, and resource allocation in response to changing conditions.
   - ![2D-4](https://github.com/Rutuja-Salunke/walmart-sales-dataset-using-KMeans/assets/102023809/d5e26692-c6bf-4cd7-b1d2-c8d17e3d61b4)

6. **3D Clustering:**
   - Extend the analysis to 3D clustering by selecting three relevant features.
   - Visualize the clusters in a 3D scatter plot for better understanding.
   - ![Screenshot 2023-12-22 163924](https://github.com/Rutuja-Salunke/walmart-sales-dataset-using-KMeans/assets/102023809/9cfa846b-3a9c-4083-928c-c5f5f0594c8b)
   - ### 6.1 3D Clustering on 'Weekly_Sales', 'Temperature', 'Fuel_Price' :
   - In the 3D clustering analysis involving 'Weekly_Sales,' 'Temperature,' and 'Fuel_Price,' the objective is to examine the interplay between weekly sales, weather conditions, and fuel prices at Walmart stores. Employing the KMeans clustering algorithm in a three-dimensional space, the dataset is segmented into clusters based on similarities in these three key factors. The resulting clusters offer insights into how variations in temperature and fuel prices contribute to distinct patterns in weekly sales. This 3D clustering analysis provides Walmart with a nuanced understanding of the relationships between sales performance and environmental and economic factors, guiding strategic decisions related to promotions, inventory management, and resource allocation.
   - ![newplot](https://github.com/Rutuja-Salunke/walmart-sales-dataset-using-KMeans/assets/102023809/2d434cd3-338e-402b-8446-b275297867ba)
   - ### 6.2 3D clustering on 'Holiday_Flag', 'Temperature','CPI' :
   - In the 3D clustering analysis involving 'Holiday_Flag', 'Temperature,' and 'Consumer Price Index (CPI),' the goal is to explore the joint influence of holidays, weather conditions, and economic indicators on Walmart store sales. Using the KMeans clustering algorithm in a three-dimensional space, the dataset is partitioned into clusters based on similarities in these three factors. The resulting clusters provide a holistic understanding of how holidays, temperature variations, and CPI collectively impact consumer behavior and sales trends. This 3D clustering analysis equips Walmart with insights to tailor strategies for specific market conditions, ensuring effective resource allocation, targeted marketing, and optimized sales performance.
   - ![newplot (1)](https://github.com/Rutuja-Salunke/walmart-sales-dataset-using-KMeans/assets/102023809/ac892ff2-06b6-4e2e-ac45-f7a1c615d1f7)



7. **Customer Segmentation:**
   - Perform customer segmentation using features like Weekly_Sales, Temperature, Fuel_Price, CPI, etc.
   - Apply KMeans clustering to group customers based on similar purchasing behavior.

8. **Evaluation Metrics:**
   - Evaluate the effectiveness of clustering using metrics such as Inertia and Silhouette Score.
   - These metrics provide insights into the compactness of clusters and the separation between them.

9. **Visualization:**
   - Utilize visualization tools like Matplotlib, Seaborn, and Plotly to create informative plots and charts.
   - Present the clusters and patterns discovered in a visually appealing manner.

10. **Conclusion and Recommendations:**
    - Summarize the key insights obtained from the analysis.
    - Provide recommendations for Walmart based on the identified clusters, such as targeted marketing strategies, store-specific initiatives, and inventory management improvements.


