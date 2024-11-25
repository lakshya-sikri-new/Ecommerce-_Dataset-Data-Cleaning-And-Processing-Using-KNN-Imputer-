# Laptop Web Scraping  (Data Cleaning And Processing With KNN Imputer)
This project involves a comprehensive approach to cleaning and preprocessing an electronics product dataset. The dataset includes a wide variety of features, such as brand names, prices, customer ratings, screen sizes, processor details, and release years, among others. The data is riddled with challenges such as missing values, inconsistent formats, incorrect data types, and significant outliers, making it unsuitable for analysis or modeling in its raw form. By implementing advanced data cleaning techniques and preprocessing methods, this project aims to prepare the dataset for further analysis, visualization, and machine learning applications.


# Problem Statement
In today’s competitive e-commerce landscape, delivering accurate product recommendations and implementing effective pricing strategies are critical to enhancing customer satisfaction, increasing sales, and optimizing inventory management. However, these objectives are often hindered by the challenges posed by incomplete, inconsistent, and inaccurate product data. Poor data quality not only impacts customer experience but also impairs decision-making processes, affecting key areas such as recommendations, pricing, and inventory forecasting.

This project addresses these challenges within a dataset of electronic products, which includes attributes such as brand, price, ratings, processor specifications, and storage capacities. The dataset reveals several issues that require immediate attention. Missing data in fields such as Rating, Processor, Screen Size, and Manufacturer Color makes it difficult to assess the overall quality and characteristics of the products, ultimately affecting the platform’s ability to recommend items that align with customer preferences. Inconsistent formats further exacerbate the problem, with fields like Price containing a mix of numeric and string values, preventing accurate filtering, pricing analysis, and decision-making.


# Objective
The primary goal of this project is to enhance the e-commerce platform’s capability to recommend products, optimize pricing, and improve inventory management by cleaning and standardizing the dataset. A key objective is to enable personalized and accurate product recommendations by addressing missing values and standardizing product features, ensuring that customers receive suggestions that align with their preferences, such as price range, brand, or processor type.

Another critical objective is to develop a robust and dynamic pricing strategy by handling inconsistent and outlier values in the Price column. This will ensure that prices reflect market trends and product demand while maintaining competitive advantage and profitability. By identifying and removing duplicate product entries, normalizing product attributes, and addressing inconsistencies, the project also aims to improve inventory forecasting. This will enable the platform to efficiently stock popular products while avoiding excess inventory, leading to more precise inventory management.

# About the Dataset
The dataset comprises product-related information from the electronics domain. It contains fields such as Brand, which specifies the manufacturer; Price, indicating the cost of the product; and Rating and Ratings Count, which reflect customer reviews. Other attributes include technical specifications like Processor, Screen Size, Maximum Resolution, and GPU. Additionally, categorical fields like Condition and Country Region Of Manufacture provide further context about the products. The dataset also features several challenges, including inconsistent formats in Price and Release Year, significant outliers in numerical fields, and varying levels of missing data across columns.

# Process Overview
The data cleaning process began with handling missing values using a combination of SimpleImputer for mean and median imputations and KNNImputer for multivariate imputation. This ensured that missing values were addressed systematically based on column relationships. Next, the dataset was reformatted by removing symbols from fields like Price and converting it to an integer type. Data type conversion was performed to align columns such as Release Year and Ratings Count with their appropriate types. Outlier detection and management were carried out using statistical methods like Interquartile Range (IQR) and Z-scores, which helped to cap extreme values and ensure the stability of the dataset. Duplicate rows were identified and removed to eliminate redundancy, and categorical values were standardized to maintain consistency.


# Tools and Libraries
This project utilized Python as the primary programming language. Data manipulation and cleaning were performed using pandas and numpy. For missing value imputation, SimpleImputer and KNNImputer from the sklearn.impute module were employed. Outlier handling relied on statistical tools from the scipy library, while data visualization for outlier detection used matplotlib and seaborn. Regular expressions (re) were used for cleaning textual data in fields like Price.

# Results
By the end of the cleaning process, the dataset was transformed into a clean, structured format. Missing values were imputed, numerical columns were free of extreme outliers, and all fields were formatted consistently. The cleaned dataset is now suitable for exploratory data analysis, statistical modeling, and machine learning. It can also be used to gain actionable business insights into product pricing, customer preferences, and manufacturing trends.




