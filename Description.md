# Project Goals and Background

In the 21st century, huge amounts of data are generated, especially in technology-driven sectors like retail. Walmart, a major retail player, relies on data to predict future sales and compete globally. With over 11,000 stores worldwide, understanding customer behavior is vital. This research aims to forecast Walmart's sales based on historical data, considering factors like temperature and holidays. By analyzing past data and using big data analytics, Walmart can optimize sales, promotions, and resources, ensuring competitiveness and profitability in the dynamic market.

# Purpose Statement
This study aims to predict how much Walmart will sell each week based on data collected from 45 different stores across the country, spanning from 2010 to 2013. The dataset includes information about store size, type, departments, weekly sales, and whether it's a holiday week. We're looking at various factors like Consumer Price Index, temperature, fuel prices, promotions, and unemployment rates to figure out if they influence weekly sales. It helps understand the patterns and connections between sales and these factors.
This study also includes an extensive exploratory data analysis on the provided Walmart dataset to understand the following:
• Identifying store as well as department-wide sales in Walmart
• Identifying sales based on store size and type
• Identifying how much sales increase during holidays
• Correlation between the different factors that affect sales
• Average sales per year
• Weekly sales as per region temperature, CPI, fuel price, unemployment
# Exploratory Data Analysis

Before predicting Walmart's weekly sales, it's crucial to deeply understand the dataset. Exploratory Data Analysis (EDA) is like a detective work, examining patterns and trends in the data that might not be obvious. Through visualizations and tools like 'inspectdf' and 'glimpse' in R, we investigate the dataset's structure, identifying missing values, numeric/categorical distributions, and correlations. Using packages like 'ggplot2' and 'matplotlib', we create visuals showing sales patterns by store, department, holidays, regions, and factors like CPI, fuel price, etc. These visuals help us uncover insights for future predictive modeling.
We use a helpful package function, 'isna()', to identify missing values in our dataset. Except for the file, there are no missing values in other datasets. The missing values in 'features' are mainly in columns related to holiday promotions, which is common due to seasonal pricing during holidays (mostly from November to January).

