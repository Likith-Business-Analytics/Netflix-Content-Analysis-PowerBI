# Netflix-Content-Analysis-PowerBI
An interactive Power BI dashboard that provides deep insights into Netflix’s catalog of Movies and TV Shows. It analyzes show types, release trends, ratings, directors, and country-wise distribution using various DAX measures and data cleaning techniques.

---

## Objective

The primary objective of this project is to **analyze Netflix’s global content library** and uncover patterns related to:

* Growth of Netflix titles over time
* Distribution of Movies vs TV Shows
* Content availability across countries
* Director and rating-based content trends
* Key metrics that summarize platform expansion

This dashboard enables users to explore the dataset using filters such as **Show Type, Release Year, and Country**, allowing for a fully interactive analytical experience.

---

## Dataset

**Source:** Public Netflix Titles Dataset (Kaggle)

**Dataset :** <a href="https://github.com/Likith-Business-Analytics/Netflix-Content-Analysis-PowerBI/blob/main/netflix_titles.csv"> netflix_titles <a/>

**Key Columns Used**

* `show_id` – Unique identifier
* `type` – Movie / TV Show
* `director` – List of directors (cleaned to extract first director)
* `country` – Country of production (cleaned to first country name)
* `date_added`
* `release_year`
* `rating`

---

## Technology Used

* Power BI Desktop
* Power Query (Power BI Transform Data)
* DAX (Data Analysis Expressions)
* CSV Dataset

---

## Key Performance Indicators (KPIs)

The dashboard uses DAX measures to calculate essential KPIs:

**DAX Measures Created**

* Total Shows
* Total Movies
* Total TV Shows
* Total Directors

**Displayed KPIs**

* Total Shows
* Total Movies
* Total TV Shows

---

## Data Cleaning Process (Transform Data)

Extensive cleaning was done using Power Query:

**1. Extract First Country Name**

The `country` column often contained multiple countries separated by commas.
Used: **Extract → Text Before Delimiter “,”**
→ Result: Single primary country for each title.

**2. Extract First Director**

Similar cleaning applied to the `director` column to ensure only 1 director is analyzed.

**3. Trim & Clean Data**
* Standardized text formats
* Ensured proper Date and Duration formatting

**4. Data Modeling**

Used a single clean fact table with DAX measures for calculations.

---

## Process / Workflow

1. Imported dataset (`netflix_titles.csv`) into Power BI
2. Cleaned and transformed data using Power Query
3. Created DAX measures for KPIs
4. Built interactive visualizations:

   * Donut charts
   * Bar charts
   * Line chart (Title growth over time)
   * Global map (Country distribution)
5. Added filters for Show Type, Release Year, and Country
6. Designed a dark-themed Netflix-style dashboard
7. Published final PBIX + documentation

---
## Dashboard

<img width="1151" height="647" alt="image" src="https://github.com/user-attachments/assets/459dacc1-72e8-4142-aff9-c652ce99c6c6" />

---

## Insights

Some important insights obtained from the analysis:
* **Movies dominate Netflix**, making up ~70% of total content.
* **TV Shows account for ~30%**, showing a balanced but Movie-heavy library.
* There is a **sharp rise in Netflix content after 2015**, indicating aggressive expansion.
* Rating distribution shows **TV-MA** and **TV-14** as the most common ratings.
* The United States, India, UK, and Canada appear as top content-producing countries.
* A large number of titles have **no assigned director** due to missing metadata.

---

## Conclusion

This Power BI dashboard provides a complete 360° analysis of Netflix’s content library.
It helps understand:
* How Netflix's catalog has evolved
* How content varies by country and rating
* Trends in Movies vs TV Shows
* Global distribution patterns
* Metadata gaps (directors, countries, ratings)


If you want, I can also help you format it using **Markdown styling**, add emojis, or structure it in a more premium GitHub style.
Would you like a **GitHub repository name + tags + description** too?
