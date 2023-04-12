## Video Game Analysis for a New Game Development

This is my first Data Analytics project.

#### 1. DESCRIPTION
This analysis identifies potential opportunities for new game development for the upcoming quarter and optimize selling strategies. It uses techniques to help better decision-making for the video game development for the next quarter.

#### 2. Dataset Description
Downloaded Data from [Kaggle Video Game Sales](https://www.kaggle.com/datasets/gregorut/videogamesales)
Fields include:
Rank - Ranking of overall sales
Name - The games name
Platform - Platform of the games release (i.e. PC,PS4, etc.)
Year - Year of the game's release
Genre - Genre of the game
Publisher - Publisher of the game
NA_Sales - Sales in North America (in millions)
EU_Sales - Sales in Europe (in millions)
JP_Sales - Sales in Japan (in millions)
Other_Sales - Sales in the rest of the world (in millions)
Global_Sales - Total worldwide sales

#### 3. Data Preparation
```pandas, numpy```
- Preporcessing
  - Match units to Million in sales
  - Preprocess nulls 
- Feature Engineering
  - classify by publisher
  - Append/join extra column to regroup by platform(handheld, home, PC) and create a new column named "Multiplatform"
  - Add a new column named "Total_Sales" by summing up all the Sales
- Exploratory Data Analysis
Hypothesis: The genre of the preferred game varies by region. (True)

#### 4. Data Visualization
```matplotlib, seaborn```

#### 5. Conclusion
Action: Red Ocean
Genre: Shooter
Action takes a bigger amounts than Shooter does but it has already been considered to be red ocean.
In addition, although Sports was on the high sales, it recently became Sports: recent sales is not that good

The sales graph is flowing in a similar direction to NA sales. Thus, if the shooter genre is released in North America, additional profits from European games can also be expected.

Develop the video game in a PS4 and PC cross-platform expects high profits.

#### 6. Challenges
The dataset used was not up-to-date, as it only included data up to 2016. Despite this limitation, I was able to derive valuable insights and make informed decisions by carefully analyzing the available data and accounting for any potential changes or trends that may have occurred since then.
- Accumulated data high in PS3 but for now, according to the current video game market, PS4 is more -selling than ps3
