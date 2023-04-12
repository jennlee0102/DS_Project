## Video Game Analysis for a New Game Development

This is my first Data Analytics project.

#### 1. Purpose
The purpose of this analysis is to identify potential opportunities for new game development and optimize selling strategies for the upcoming quarter. By utilizing various techniques, this analysis aims to provide insights to aid in better decision-making for video game development in the next quarter.

#### 2. Dataset Description
Downloaded Data from [Kaggle Video Game Sales](https://www.kaggle.com/datasets/gregorut/videogamesales) <br>
Fields include: <br>
Rank - Ranking of overall sales <br>
Name - The games name <br>
Platform - Platform of the games release (i.e. PC,PS4, etc.) <br>
Year - Year of the game's release <br>
Genre - Genre of the game <br>
Publisher - Publisher of the game <br>
NA_Sales - Sales in North America (in millions) <br>
EU_Sales - Sales in Europe (in millions) <br>
JP_Sales - Sales in Japan (in millions) <br>
Other_Sales - Sales in the rest of the world (in millions) <br>

#### 3. Data Preparation
```pandas, numpy```
- Preporcessing
  - Match units to Million in sales
  - Preprocess nulls
  - Remove the data before 2000
- Feature Engineering
  - classify by publisher
  - Append/join extra column to regroup by platform(handheld, home, PC) and create a new column named "Multiplatform"
  - Add a new column named "Total_Sales" by summing up all the Sales
- Exploratory Data Analysis
  - Hypothesis 1: There may be a discernible pattern based on the year, including factors such as genre and platform. (True)
  - Hypothesis 2: The preferred game genre varies depending on the region. (True)

#### 4. Data Visualization
```matplotlib, seaborn```<br>
See [ipynb file](https://github.com/jennlee0102/DS_Project1/blob/main/Video_Game_Analysis.ipynb)

#### 5. Conclusion
Action games generate more revenue than Shooter games, but the Action genre is already considered a saturated market (red ocean) and the average sale of **Shooter** is the highest among all genres. Furthermore, although the Sports genre had high sales in the past, recent sales have been lackluster. The sales trend in North America is similar to that in Europe, so launching a Shooter game in **North America** could result in additional profits from European sales. Developing the game for **both PS4 and PC platforms** is expected to yield high profits.

#### 6. Challenges
1. The dataset used was not up-to-date, as it only included data up to 2016. Despite this limitation, I was able to derive valuable insights and make informed decisions by carefully analyzing the available data and accounting for any potential changes or trends that may have occurred since then.
- While the accumulated total sales for PS3 was high, it's important to note that the available data only covers the beginning of the PS4. A line graph analyzing the best-selling platforms reveals that PS3 sales have been declining since 2011, while PS4 sales have been on the rise since its release.

2. When entering a new market, it is important to conduct research on various factors such as the country's culture, policies, laws, regulations, and economic conditions. This will help to determine the feasibility of entering the market and the best approach to take. Factors such as consumer behavior, local customs, and language barriers can also affect the success of entering a new market. It is important to understand these factors and tailor the marketing and business strategies accordingly to ensure success.
