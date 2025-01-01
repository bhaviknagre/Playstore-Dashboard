# Playstore Analysis

## Project Overview
This project focuses on analyzing an app dataset containing various attributes such as app categories, ratings, reviews, installs, and more. The goal is to provide actionable insights regarding the app market, user sentiment, and trends based on the available data. The insights will be visualized in a Power BI dashboard that will help in making data-driven decisions.

## Dataset Description
The dataset consists of multiple columns that describe the properties of different apps. Some of the key columns are:

- **App**: Name of the app.
- **Category**: Category the app belongs to (e.g., Games, Social, etc.).
- **Rating**: Average user rating of the app.
- **Reviews**: Number of reviews for the app.
- **Size**: Size of the app in MB.
- **Installs**: Number of times the app has been installed.
- **Type**: Paid or Free status of the app.
- **Price**: Price of the app (only for paid apps).
- **Content Rating**: Rating given based on the app's content (e.g., Everyone, Teen, etc.).
- **Genres**: Genre of the app (e.g., Action, Adventure, etc.).
- **Last Updated**: Date the app was last updated.
- **Current Ver**: The current version of the app.
- **Android Ver**: Minimum Android version required for the app.

## Steps to Analyze the Data
### 1. Data Preprocessing
The initial dataset was cleaned to handle missing values and format inconsistencies. Key preprocessing steps included:

- Handling missing values by imputing or replacing them with meaningful data.
- Transforming categorical variables using encoding methods such as `pd.get_dummies` and `LabelEncoder`.
- Converting install values (e.g., "50+", "1,000+") to numeric data for analysis.

### 2. Key Insights from the Data
- **App Distribution by Category**: Analyzed the distribution of apps across different categories and identified the most popular categories.
- **App Pricing and Revenue**: Investigated the relationship between app price, category, and revenue generation for paid apps.
- **Sentiment Analysis**: Sentiment analysis was performed on app reviews to classify the sentiment into Positive, Neutral, and Negative categories.
- **Reviews and Ratings Distribution**: Examined the distribution of app ratings and the total number of reviews.
- **Install Trends**: Analyzed the trend of app installations and compared free vs. paid apps in terms of their install count.

### 3. Power BI Dashboard
A Power BI dashboard was created to visualize the key insights derived from the data. The dashboard includes the following visualizations:

#### KPIs:
- **Total Apps Count**: Displays the total number of apps in the dataset.
- **Average Rating**: Shows the average rating of all apps.
- **Total Reviews**: Total number of reviews across all apps.
- **Revenue from Paid Apps**: The sum of prices for all paid apps.
- **Top Category by App Count**: The category with the highest number of apps.
- **Top Rated App**: The app with the highest rating.
- **App Installations Distribution**: Displays the total number of installations across all apps.

#### Charts:
- **Bar Chart**: App Count by Category.
- **Pie Chart**: Distribution of Free vs Paid Apps.
- **Line Chart**: Rating Trend by Last Updated Date.
- **Stacked Column Chart**: Reviews and Installs by Category.
- **Histogram**: Distribution of Ratings (Bins like 0-1, 1-2, ..., 4-5).
- **Tree Map**: Revenue by Category (for Paid Apps).

#### Slicers:
- **Category**: Allows users to filter the data by app category.
- **Type (Free vs Paid)**: Filters data to show either free or paid apps.
- **Content Rating**: Filters based on the app's content rating (e.g., "Everyone", "Teen", etc.).

### 4. Insights from the Dashboard
- **Category Performance**: Identify the best-performing categories in terms of app count, reviews, and installs.
- **Sentiment Distribution**: Visualize the sentiment (positive, neutral, negative) of app reviews and correlate with the app's performance.
- **Top Categories for Paid Apps**: Identify which categories contribute the most to revenue from paid apps.
- **Install Trends**: Gain insights into how app installs vary across different categories and types (free vs. paid).
- **Rating Distribution**: Understand how app ratings are distributed across different categories and types.

## Conclusion
This project offers valuable insights into the app market, highlighting the trends, performance metrics, and user sentiments that can guide app developers, marketers, and business decision-makers. The Power BI dashboard provides a user-friendly interface to interact with the data and derive insights to improve business strategies.

## Future Work
- **Sentiment Analysis Improvement**: Improve sentiment classification using advanced NLP models for better accuracy.
- **Price Optimization Model**: Implement a predictive model to recommend optimal pricing for apps based on various features.
- **User Demographics**: Include user demographics data for further segmentation analysis and targeted marketing strategies.

## Requirements
- **Pandas**: For data manipulation.
- **Power BI**: For creating interactive dashboards.
- **Scikit-learn**: For any machine learning tasks (if applicable).
- **Matplotlib/Seaborn**: For data visualization.
- **LabelEncoder**: For encoding categorical variables.
