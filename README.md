# Pixar-Films-Legacy 
Maven Pixar Challenge
## Objective: 
To analyze and showcase the legacy of Pixar Films over the last 30 years through effective storytelling, using an infographic or interactive visual. 
## Dataset: 
CSV files with structured information about every Pixar film from Toy Story (1995) to Inside Out 2 (2024). It lists each film’s creators (storywriters, screenwriters, directors, composers, and producers), budget, box-office earnings, critic ratings, Oscar nominations, genres, audience rating and more. 
## Approach: 
### Data Cleaning: 
- Used SQL to clean and prepare data. Formatted the release_date column to (yyyy-mm-dd), for SQL to take it as a date data type.
- Found a missing value for budget for a film (**_Luca_**) and since it wasn't even mentioned in the official site I kept the missing value and accounted for it in my calculations.
- Identified incorrect entries, the same name for all 6 roles for 2 films- **_Brave_** and **_Luca_** in pixar_people table. Updated the table by replacing those entries with the correct names.
- Corrected the spelling of the creators' names - Ronnie del Carmen for **_Inside Out_** and Mycheal Danna for **_The Good Dinosaur_**
Imported the tables in Power BI to visualize the data. Let's look at the dashboard I created.
### Dashboard: 
I divided the dashboard into 5 pages - Genre, Box Office Performance, Ratings, Academy and Creators since these are the key aspects of the legacy and help analyze the effect of the films.
#### Genre: 
- For Subgenre Trend I calculated the percentage of films and used a scatter plot to show film percentage in a subgenre over the year.
![Image](https://cdn.mavenanalytics.io/public/profile/b811f350-c001-70a4-257f-2ad6df4e78f5/projects/Screenshot-2025-04-02-043341.png)
#### Insights: 
- All 28 films have Adventure and Animation as the common genres and Computer Animation as the common subgenre.
- Pixar started out with Buddy Comedy (Toy Story) but it's trend is declining- there is no film after 2015 with Buddy Comedy subgenre.
- Meanwhile, Coming-of-Age subgenre is on a growing trend.


