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
### Genre: 
- For Subgenre Trend I calculated the percentage of films and used a scatter plot to show film percentage in a subgenre over the year.
![Image](https://cdn.mavenanalytics.io/public/profile/b811f350-c001-70a4-257f-2ad6df4e78f5/projects/Screenshot-2025-04-02-043341.png)
#### Insights: 
- All 28 films have Adventure and Animation as the common genres and Computer Animation as the common subgenre.
- Pixar started out with Buddy Comedy (Toy Story) but it's trend is declining- there is no film after 2015 with Buddy Comedy subgenre.
- Meanwhile, Coming-of-Age subgenre is on a growing trend.
### Box Office Performance:
Calculated the Gross Profit and ROI%(Return on Investment) as performance indicators. A film is considered-  
financially successful if the ROI% >100% or ROI > 2, or simply, if it earned more than twice its budget.  
ROI% = 0% (or ROI = 1) is the break even point indicating no gain no loss, meaning it earned exactly what it cost to make.  
ROI% < 0% (or ROI < 1) means the film lost money, it's considered a failure.  
![Image](https://cdn.mavenanalytics.io/public/profile/b811f350-c001-70a4-257f-2ad6df4e78f5/projects/Screenshot-2025-04-02-051215.png)  
#### Insights:  
- Box Office earning, Gross Profit and ROI%(Return on Investment) are at the lowest during 2020,2022 which was the Pandemic period. Then it recovered and **_Inside Out 2_** in 2024 brought an all time high box office earning of $1.7B.
- **_Toy Story (1995)_** still leading in ROI% is Pixar's most successful film commercially (and rating wise too).
- 3 films showed negative ROI% (loss)- **_Soul_**,  **_Onward_**,  **_Turning Red_**, **_Turning Red_** being the most unsuccessful film commercially.
### Ratings: 
Analyzed the Rotten Tomatoes, Metacritic, and IMDb scores and to see if the critics ratings and audience ratings match I have used a dumbbell chart.  
![Image](https://cdn.mavenanalytics.io/public/profile/b811f350-c001-70a4-257f-2ad6df4e78f5/projects/Screenshot-2025-04-02-052901.png)  
#### Insights:  
- Overall, Rotten Tomatoes has higher scores than the Metacritic and IMDb score.
- The drop in all 3 scores is the largest for **_Cars2_** in 2011 making it the least rated film overall.
- The Pandemic didn't have any effect on the ratings.
- **_Toy Story (1995)_** is the highest rated film overall.
- Critics score is generally higher than audience score. Only 3 films, **_Cars 2_**, **_Cars 3_**, **_Elemental_** were rated higher by the audience than critics.
- The biggest rating gap was for **_Turning Red_**, which was also the least profitable.
### Academy:  
To visualize the films, nominations, win, award categories in one place I used a matrix.  
Also used a stacked column chart with year to show if the films win all the nominations. Only **30%** result in win.  
![Image](https://cdn.mavenanalytics.io/public/profile/b811f350-c001-70a4-257f-2ad6df4e78f5/projects/Screenshot-2025-04-02-064746.png)  
#### Insights:  
- Academy only introduced the Animated Feature category in 2001, but it brought the most nominations and wins for Pixar films.
- **_Wall-E_** had the most nominations(6).
- Pixar's number of nominations and win % has been declining over the years with its last win in 2020 for **_Soul_**.
### Creators:  
![Image](https://cdn.mavenanalytics.io/public/profile/b811f350-c001-70a4-257f-2ad6df4e78f5/projects/Screenshot-2025-04-02-064951.png)  
#### Insights: 
- The top 10 creators by number of roles show Andrew Stanton on top with 20 roles, followed by Pete Docter with 14.
- Andrew Stanton worked 80% of the time as a screenwriter or storywriter.
- Andrew Stanton and Randy Newman have both worked in most number of Pixar films i.e. 9, followed by Michael Giacchino with 8 films.
- 2 creators with the most number of roles (4) they have taken on- Andrew Stanton, Angus MacLane.
## Conclusion:  
Pixar’s legacy is built on emotional storytelling, genre innovation, and a core group of creative leaders. This analysis reveals what has driven its success—and what hasn’t—helping Pixar understand audience trends-what resonates with them and creative impact. These insights can guide smarter decisions that lead to more financially successful, critically acclaimed, and award-winning films.

[Project Submission in Challenge](https://mavenanalytics.io/project/29992)
