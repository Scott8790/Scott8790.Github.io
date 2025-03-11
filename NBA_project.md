<img src="NBA_project_visuals/NBA_titleimage.png?raw=true"/>

# Scoring Big: What My NBA Season Analysis Taught Me About Data and Player Performance

As a sports fan, I often find myself glued to the screen during live games, cheering for my favorite teams and players. But it's not just the thrill of the game that excites me; it's the numbers, the stats, and the stories they tell. Analyzing player performances has always piqued my interest, leading me to dive into a project that combined my passion for sports with my love for data. I would like to preface my data analysis by stating that I am not the biggest fan of basketball and that my knowledge of the game and its players is minimal at best. However, I am open to the challenge of learning some ins and outs of basketball and looking into some player stats to see what went on in this 2021-2022 season.

## Why THIS Project?

The motivation behind this project was personal. I have always enjoyed comparing individual player stats and wondering how teams can improve. I wanted to figure out which positions had the highest three-point shooting percentages, identify ideal free-agent signings, and highlight the top scorers across teams. This blend of sports and analytics felt unique and special to me, as I believed it could help teams make informed decisions for their rosters. I put myself in the mind of a team manager and asked questions that I would think they would want answers to in order to improve their team's performance for the upcoming season. Feel free to look at my analysis here on tableau public.

## What Readers Will Gain

In this article, you'll learn about my key findings from the NBA season, including surprising statistics, standout players, and insights that can inform team strategies. Whether you’re a sports fan, a budding data analyst, or just curious about how numbers can tell a story, there’s something here for you!

## Key Takeaways

The analysis revealed Atlanta's centers had an unusually high three-point shooting percentage, primarily due to one player.
Nikola Jokic emerged as a standout player with impressive stats, making him a prime target for teams looking to bolster their rosters.
Questions regarding player performance should always be accompanied by a "why" to uncover deeper insights.

## Dataset Details

For this project, I utilized a dataset from [basketball-reference.com](https://www.basketball-reference.com/leagues/NBA_2022_totals.html), which contained over 800 rows and 30 columns of individual player stats for the 2021-2022 NBA season. This dataset was ideal because it provided a comprehensive overview of player performances, allowing for in-depth analysis and insights.

## Analysis Process

My analysis involved several steps, including data cleaning, transformation, and visualization. I focused on creating visual representations, such as a heat map, bubble plot, stacked bar chart, and a treemap to make the data more digestible. All of these charts were created in Tableau.

## Visuals and Insights


<img src="NBA_project_visuals/heatmap_3p%.png?raw=true"/>

Heatmap: Team 3-pt % split by position. Outliers of UTA C and ATL C are interesting due to the lack of attempts at shooting 3-pointers. Atlanta had only one player actively shooting 3 point shots. Utah only had one player attempt to shoot a 3-pointer, Rudy Gobert, and that was only four attempts. Zero of his attempts made it through the net. It is important to take another look at the outliers in your data and try to make sense of it or to see if there was an error in the data. The more realist 3P% as you can see in the chart is in the 30% range and that goes for all 5 positions interestingly enough. This tells me that all positions in basketball have a good chance to attempt a 3-pointer. 


<img src="NBA_project_visuals/bubble_chart.png?raw=true"/>

Bubble Plot: This chart displayed individual player stats for assists, points, and rebounds. Jokic stood out as an exceptional performer, accumulating 584 assists, 2004 total points, and 1019 total rebounds. Any team looking to strengthen their lineup should consider him! I found it interesting to see LeBron James's dot smaller than most of the other centers. This tells me he does not focus on rebounds as much as other centers. I also found it interesting to see quite a few other players with more total points than him since he is constantly considered to be one of the greatest players in NBA history. Perhaps his older age is affecting his performance or this could be an off year for him? Who knows, but it is worth more investigation for sure if you were going to consider adding him to your roster.


<img src="NBA_project_visuals/stacked_barchart.png?raw=true"/>

Stacked Bar Chart: Shows each team's top scorers where the top players are broken down by color and size based on their total points. It is interesting to see which teams have one clear top shooter and which ones have two or three strong shooters. There are more players than there are colors so there will be repeated colors on this chart but it is more important to see how big each piece is to see their total points scored and see their performance for the season. Any recruiter for any team would want to look at this chart and see who could they trade or pick up if they wanted to add another great player to their team.


<img src="NBA_project_visuals/treemap_assists.png?raw=true"/>

Treemap: Shows assists split by position. Point Guards (PG) have the most assists due to the nature of that position. It is their job to pass the ball around the court in order to create and make plays. This position passes the ball more than the others. James Harden had the most assists with 1334. Trae Young was second with 737 assists and Chris Paul was third with 702 assists. The team manager wants to know about the other positions as well and see their assists. For the Power Forward (PF), Domantas Sabonis was the leader with 646 assists. For the Strong Forward(SF), Khris Middleton takes the top spot with 358 assists. For the Strong Guard(SG), Derrick White leads with 732 assists. Then finally for the Center(C), Nikola Jokic takes home the gold medal with 584 assists. Any of these players would make a significant improvement to the team's overall success and should be considered.

## Main Takeaways

Through this project, I learned the necessity of digging deeper into the data to understand the "why" behind the numbers. One surprising outcome was Atlanta's high three-point percentage for centers, predominantly influenced by Gorgui Dieng’s shooting prowess. His impressive 42.6% from beyond the arc skewed the results, prompting me to think critically about the data and its implications. It was skewed because he was the only player actively shooting for 3's where the other two centers were not. Anomalies, like Atlanta's three-point shooting percentage for centers, taught me to always ask questions and seek clarity. Ultimately, using reliable data allows analysts to better support stakeholders’ needs. Don't just accept what you hear as facts all the time. I believe the data every time over someone's opinions or blind assumptions. Find the truth for yourself within the data and come up with your own insights, you will feel better for it!

## Conclusion and Personal Reflections

This analysis was not without its challenges. At times, the overwhelming amount of data I knew very little about felt daunting. However, I discovered that maintaining a curious mindset transformed these challenges into learning opportunities. This project has reshaped my perspective on data analysis, making me appreciate the stories behind the stats even more. This project has inspired me to do a similar analysis for baseball or football as I do prefer them over basketball. 

I invite you to connect with me on [LinkedIn](https://www.linkedin.com/in/smsilvey/). If you or someone you know is looking to hire a data analyst, let’s chat! I’d love to hear your thoughts or answer any questions you may have about this project or data analysis in general.

[<img src="images/Button.jpg?raw=true"/>](/index.md).
