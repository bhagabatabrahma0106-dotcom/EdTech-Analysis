# EdTech-Analysis

📊 EdTech App Market Analysis
📌 Project Overview

This project presents a comprehensive data analysis of the EdTech mobile app market. The goal is to analyze app performance, user engagement, and market trends using various data analytics techniques.

The analysis focuses on key metrics such as installs, ratings, reviews, scores, content ratings, and Android versions to understand what factors influence app popularity and performance. The project follows a complete end-to-end data analytics workflow, including data cleaning, exploratory data analysis (EDA), SQL-based insights, machine learning clustering, and dashboard visualization.

This project demonstrates how raw data can be transformed into actionable business insights using modern data analytics tools.

🎯 Objectives

The main objectives of this project are:

Analyze install distribution and rating patterns of EdTech apps

Identify top-performing apps by installs

Compare apps with ads vs without ads

Identify most targeted Android versions

Discover developers with the most apps

Segment apps using machine learning clustering

Create an interactive Power BI dashboard for visual insights

📂 Dataset

The dataset contains information about various EdTech applications available on the Play Store.

Key Features in Dataset

App Name

Installs

Score (Rating)

Reviews

Ratings Count

Content Rating

Android Version

Developer

Ads availability

These attributes help analyze app popularity, user satisfaction, and market trends.

🛠️ Tools & Technologies Used
Data Analysis

Python

Pandas

NumPy

Matplotlib

Seaborn

Database & Querying

SQL Server

Machine Learning

K-Means Clustering

Data Visualization

Power BI

Data Preparation

Excel / CSV

📊 Project Workflow
1️⃣ Data Cleaning

The raw dataset was cleaned and prepared for analysis using Python.

Cleaning steps included:

Handling missing values

Converting installs and reviews into numeric format

Removing duplicates

Formatting columns for analysis

📈 Exploratory Data Analysis (EDA)

EDA was performed to understand data patterns.

Installs Distribution

Most apps have low to medium installs

A few apps have extremely high installs

Score Distribution

Most app scores fall between 3.5 and 4.5

Scores are fairly balanced with few outliers

🗄️ SQL Analysis

SQL queries were used to extract key insights from the dataset.

1️⃣ Top 10 Apps by Installs

This query identifies the most downloaded apps in the dataset.

Example results:

Duolingo

BYJU'S – The Learning App

Unacademy Learner App

These apps dominate the EdTech market in installs.

2️⃣ Average Score: Apps With Ads vs Without Ads

Result:

Contains Ads	Average Score
False	3.9
True	4.1

Insight:
Apps containing ads still maintain competitive user ratings.

3️⃣ Most Popular Android Version

Android versions most targeted by developers:

Android Version	Number of Apps
5	40
6	9
4.1	8
4	7

Insight:
Developers prioritize Android 5 compatibility due to wide device support.

4️⃣ Developer with the Most Apps

Top developers by number of apps:

Developer	Number of Apps
EduRev	5
BYJU'S	2
TeamLease EdTech	2

Insight:
Developers often focus on specific niches like exam preparation apps.

🤖 Machine Learning Analysis
K-Means Clustering

K-Means clustering was used to group apps based on performance metrics.

Features Used

Installs

Reviews

Scores

Number of Clusters

3 clusters were created.

Cluster Interpretation
Cluster	Description
Cluster 0	Low installs & low scores
Cluster 1	Medium installs & medium scores
Cluster 2	High installs & high scores
Key Insight

Top apps like Duolingo and BYJU'S fall into the high-performance cluster.

📊 Power BI Dashboard

An interactive dashboard was created to visualize key insights.

Dashboard Features

Total apps

Average scores

Total installs

Top apps by installs

Score by content rating

Clustering visualization

App release trends

Dashboard Link

🔗 https://shorturl.at/V3HUM

📌 Key Insights

1️⃣ Language learning and exam preparation apps dominate the EdTech market

2️⃣ Apps with ads still maintain strong ratings

3️⃣ Android 5 remains widely supported

4️⃣ High-performing apps show strong installs, reviews, and ratings

5️⃣ Clustering helps identify successful and struggling apps

💡 Recommendations

Developers should focus on high-demand categories like language learning and exam preparation

Improve app quality and marketing strategies to increase installs

Maintain compatibility with widely used Android versions

Study top-performing apps to identify successful strategies

🚀 Project Outcome

This project demonstrates a complete data analytics pipeline, including:

Data cleaning and preprocessing

Exploratory data analysis

SQL-based business insights

Machine learning clustering

Interactive dashboard visualization

It showcases how data analytics can help understand market trends and make data-driven decisions.

👨‍💻 Author
Bhagabata Brahma
Data Analytics Enthusiast | Python | SQL | Power BI
