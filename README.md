# Netflix Dataset Analysis

This project provides an in-depth analysis of the Netflix dataset using Python (Jupyter Notebook) and Power BI. The dataset contains information about various movies and TV shows available on Netflix, including their titles, release years, ratings, durations, and more. The analysis includes data cleaning, transformation, visualization, and dashboard creation to uncover insights about Netflix's content.

## Table of Contents
1. [Introduction](#Introduction)
2. [Dataset Overview](#Dataset_Overview)
3. [Data Cleaning and Transformation](#Data-Cleaning-and-Transformation)
4. [Visualizations](#Visualizations)
5. [Power BI Dashboard](#Power-Bi-Dashboard)
6. [Key Insights](#Key-Insights)
7. [Saving the Processed Data](#Saving-the-Processed-Data)
8. [How to Use](#How-to-Use)
9. [Libraries Used](#Libraries-Used)
10. [Dataset Source](#Dataset-Source)
11. [Author](#Author)

---

## Introduction
This project explores the Netflix dataset to answer questions such as:
- What is the distribution of content types (Movies vs. TV Shows)?
- How are content durations distributed across different ratings?
- Which countries produce the most Netflix content?
- What is the trend of content releases over the years?

---

## Dataset Overview
The dataset contains the following columns:
- **type**: Indicates whether the content is a Movie or TV Show.
- **title**: The title of the content.
- **director**: The director of the content.
- **country**: The country where the content was produced.
- **date_added**: The date the content was added to Netflix.
- **release_year**: The year the content was released.
- **rating**: The content's rating (e.g., PG, TV-MA).
- **duration**: The duration of the content (in minutes for Movies, seasons for TV Shows).
- **listed_in**: Categories or genres of the content.
- **duration-unit**: Extracted unit of duration (e.g., "min" for Movies, "Season" for TV Shows).

---

## Data Cleaning and Transformation
The following steps were performed to clean and transform the dataset:
1. **Set Index**: The `show_id` column was set as the index for better data manipulation.
2. **Remove Duplicates**: Duplicate rows were dropped to ensure data integrity.
3. **Convert Date Format**: The `date_added` column was converted to a datetime format.
4. **Extract Duration Details**: The `duration` column was split into numerical values and units (`duration-unit`).
5. **Standardize Units**: The `duration-unit` column was standardized by replacing "Seasons" with "Season".

---

## Visualizations
The following visualizations were created in the Jupyter Notebook:
1. **Distribution of Duration Units by Rating**:
    - A count plot showing how different duration units (e.g., minutes, seasons) are distributed across various content ratings.
2. **Percentage of Movies vs. Series**:
    - Calculated and displayed the percentage of Movies (in minutes) and Series (in seasons).
3. **Top Countries Producing Content**:
    - A pie chart showing the top 10 countries producing Netflix content.
4. **Content Release Trend Over the Years**:
    - A line chart showing the trend of content releases over the years.
5. **Rating Distribution**:
    - A bar chart showing the count of each rating category in the dataset.

---

## Power BI Dashboard
A Power BI dashboard (`Netflix Dashboard.pbix`) was created to provide an interactive exploration of the Netflix dataset. The dashboard includes:
- **Content Type Distribution**: A visual representation of Movies vs. TV Shows.
- **Top Countries**: A map and bar chart showing the top countries producing Netflix content.
- **Release Trends**: A timeline of content releases over the years.
- **Rating Analysis**: A breakdown of content ratings.
- **Duration Insights**: Analysis of content durations for Movies and TV Shows.

---

## Key Insights
- **Content Type Distribution**: The dataset contains both Movies and TV Shows, with Movies being more prevalent.
- **Top Countries**: The United States, India, and the United Kingdom are the top producers of Netflix content.
- **Release Trends**: The number of content releases has increased significantly over the years, peaking in recent years.
- **Duration Insights**: Movies are typically measured in minutes, while TV Shows are measured in seasons.

---

## Saving the Processed Data
The cleaned and transformed dataset was saved to a CSV file named `Netflix.csv` for future use.

---

## How to Use
1. Clone this repository and open the Jupyter Notebook.
2. Ensure the required libraries (`pandas`, `numpy`, `matplotlib`, `seaborn`) are installed.
3. Run the cells sequentially to reproduce the analysis and visualizations.
4. Open the `Netflix Dashboard.pbix` file in Power BI to explore the interactive dashboard.

---

## Libraries Used
- **pandas**: For data manipulation and analysis.
- **numpy**: For numerical operations.
- **matplotlib**: For creating static visualizations.
- **seaborn**: For creating advanced visualizations.

---

## Dataset Source
The dataset used in this analysis is named `netflix1.csv`. Ensure the file is in the same directory as the notebook before running the code.

---

## Author
This analysis was conducted by **Aso Maarooufiniyaa** using Python, Jupyter Notebook, and Power BI to explore and visualize the Netflix dataset.
