Nigeria Housing Price Exploratory Data Analysis (EDA)
Project Overview

This project performs an exploratory data analysis (EDA) on Nigerian housing price data to understand pricing patterns, identify key price drivers, and address data quality challenges commonly found in real-world real estate datasets. The analysis focuses on data exploration, cleaning, and preparation for future predictive modeling.

Objectives

The objectives of this project are to:
Explore the distribution of housing prices across Nigeria
Identify major factors influencing house prices
Detect and handle extreme outliers and skewed distributions
Clean and standardize categorical variables such as location and property type
Prepare the dataset for future regression modeling

Dataset Description
The dataset contains over 24,000 housing listings across multiple Nigerian states and towns. Each record includes information such as:
Number of bedrooms, bathrooms, toilets, and parking spaces
Property type (e.g., detached duplex, terraced house)
Town and state
House price
Each row represents a single housing listing.
Tools and Technologies

Python
Pandas
NumPy
Matplotlib
Seaborn
Jupyter Notebook
Git and GitHub

Data Quality Challenges

Initial exploration revealed several challenges:
Extreme price outliers, including unrealistically high and low values
Highly right-skewed price distribution
High cardinality in town-level location data
Inconsistent text formatting in categorical variables
These issues made raw analysis and modeling unreliable without preprocessing.

Data Cleaning and Feature Engineering

The following steps were applied:
Log transformation of house prices to stabilize the distribution
Percentile-based capping of extreme price values to reduce outlier influence
Standardization of categorical text fields (state, town, property type)
Grouping of rare towns into an "Other" category to reduce noise
Creation of cleaned numerical features suitable for future regression

Key Insights

House prices are highly right-skewed; the median price is more representative than the mean.
Location is the strongest determinant of housing prices, with properties in Abuja generally priced higher than those in Lagos and other states.
Property type influences pricing, but less significantly than geographic location.
Raw price data is unsuitable for direct modeling without transformation and outlier handling.
Reducing high-cardinality categorical features improves interpretability and modeling readiness.
## Visual Highlights

Log-Transformed Price Distribution
[Log Price Distribution](images/log_price_distribution.png)
House Prices by State
[Price by State](images/price_by_state.png)
House Prices by Property Type
[Price by Property Type](images/price_by_property_type.png)

Conclusion
This exploratory analysis highlights the importance of careful preprocessing when working with real-world housing data. By addressing skewness, extreme outliers, and categorical complexity, the dataset has been transformed into a cleaner and more reliable form.
The resulting dataset is well-prepared for future regression modeling to predict housing prices and analyze the quantitative impact of key features such as location and property type.

Project Structure
nigeria-housing-eda/
│
├── data/
│   └── nigeria_houses_data.csv
│
├── notebooks/
│   └── nigeria_housing_eda.ipynb
│
├── images/
│
├── README.md
└── requirements.txt

Author

Ernesto Ebimaro
Computer Science Student | Data Science & Analytics Enthusiast