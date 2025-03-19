<img src="mining_visuals/Title_image.png?raw=true"/>

# Into the Depths of Mining: A Data Analyst’s Journey

Have you ever stopped to think about how the shiny metals in your gadgets are extracted from the earth? Behind the scenes, there's an intricate process driven by both human ingenuity and cutting-edge technology. Recently, I had the chance to explore this fascinating world of mining through data analysis. As a fictional analyst at Metals R’ Us, I was handed a treasure trove of real-world data from a flotation plant refining iron ore. Our boss indicated to me and the team that something weird happened on June 1st and he wanted us to investigate. Little did I know, this deep dive into the numbers would teach me more than I ever expected about mining—and Python, my newfound tech sidekick. I have never used Python before until now, so follow along on my journey with Python and using it to analyze this mining data.

### Why I Took the Plunge
I’ve always been fascinated by minerals and the science behind their extraction. The complexity of these operations—how they’re monitored, tweaked, and perfected—was something I couldn’t resist. How does this stuff come from the ground and form into something that we all use in our everyday lives? This project wasn’t just a learning opportunity; it was a puzzle waiting to be solved. It combined my curiosity for minerals with my desire to sharpen my data analysis skills. And, it's my job, I was assigned this task to investigate the mining data and to examine the events of June 1st specifically and I wanted to learn how to use Python.

### What’s In It For You?
If you’re curious about how data can improve industrial processes or you’re diving into Python yourself, this article has you covered. Here, I’ll share how I tackled data challenges, uncovered meaningful insights, and visualized critical relationships that impact iron ore purity. I show the beginning fundamentals of any Python data analysis on getting it set up properly and writing some code to analyze the data.

### Key Highlights
The data on June 1, 2017, revealed nothing alarming.
An inverse relationship stood out between iron and silica concentrations—especially at 11 a.m. on the same day.
During the analysis, % Iron Concentrate consistently ranged between 62% and 68%.
Python turned out to be surprisingly user-friendly and powerful, even for someone like me just starting out with it.

### The Dataset: A World of Challenges
I worked with a dataset titled “Quality Prediction in a Mining Process,” sourced from [Kaggle](https://www.kaggle.com/datasets/edumagalhaes/quality-prediction-in-a-mining-process). Covering March to September 2017, this dataset included 24 variables, one of which was the crucial % Iron Concentrate. But, as with any real-world data, it wasn’t perfect. Sampling intervals were inconsistent, ranging from every 20 seconds to hourly, making the cleaning process a bit of a beast. Sometimes the data can only be manipulated so much before you compromise its integrity. One of the first things needed was to reformat the date column from a text string to a timestamp. This allows for better data analysis when it comes to dates. This was done by entering this code: df['date'] = pd.to_datetime(df['date'])

### My Approach
The journey began with some good old-fashioned cleaning—handling missing data and ensuring consistency. Then with Python, there are a few different methods of getting it installed to your computer but I went with DeepNote. It is a free version offered through Google's cloud services and was an easy option for me to start using Python. Once you are all set up with DeepNote, you need to upload your data CSV file. Then you want to make sure you have all the necessary libraries installed that you know you will need to do your analysis. For this project, I used Pandas, Seaborn, and Matplotlib. 




Interestingly enough, DeepNote already had these integrated within the software so the installation of these wasn't necessary but still good practice. Then these need to be imported so they will work properly with your code prompts. 




Once that is done, then you need to connect Python to the actual data. You create a variable to read your data in python. I used df = pd.read_csv('MiningProcess_Flotation_Plant_Database.csv',decimal=",") where df was short for data frame and this cleaned up the data by removing commas where the decimals were supposed to be.




Now we are ready to begin the analysis! One of the first codes I wrote was one to see how much data I was dealing with.




the first number is the number of rows and the second is the amount of columns


My boss wanted to see some summary stats for the data. he wanted to see the average, median, min, and max for every column. This can be quickly done in python with the following code:




Then came the fun part: visualizations. I needed to isolate the important rows andcolumns the boss wanted to see for this project. I created a variable for defined important columns. And for the rows, i filtered them with a boolean mask and created a new data frame df_june:




this filters the rows to only show June 1st since that is what our boss wanted info on



% Iron Concentrate is the most important variable. % Silica, Ore Pulp pH, and Flotation Column 05 Level are our important columns the boss cared about for June 1st.
 Using Python, I created scatterplots and correlation matrices to get a sense of the data’s relationships. Now, I am no scientist myself and cannot explain the relationships all that well. I'm just the analyst and my job is to present the information to the boss. It's their job to ultimately take the info I provide and come up with their own solution. They are the ones who know the ins and outs of the whole operation. I'm just the data guy. Don't shoot the messenger. Thankfully, the data visualization library Seaborn allows us to show all the scatterplots to look at all the variables.




Note the scale of the x and y axes. Nothing too alarming 
To our team's surprise, there were low correlation values between most variables—not exactly what I had expected from a mining dataset. We wanted to confirm this by running a correlation matrix to see all the correlation values.




As we can see, all correlation values are low indicating these variables don't seem to have much of a relationship.
The boss was surprised by all this and wanted to see the data to help them understand more. They wanted to see how the % Iron Concentrate changed throughout the day on June 1st. I made a line plot in Seaborn to show this.




The boss found this info useful and wanted to see line plots for the other important variables as well. I created a for loop to create the other graphs since the units of measure are very different for each variable. When dealing with percentages, pH levels, and flotation levels, it is best to have separate graphs to better show the trends throughout the day.




for loop code






Lineplots for all 4 important column variables


Revealing the Insights
Here’s where things got interesting:

Dataset Dimensions: Key variables like iron concentration, silica concentration, ore pulp pH, and flotation column levels all took center stage. Histograms revealed trends, with iron and silica values remaining steady while flotation levels fluctuated slightly.
Iron Concentration Changes: A line plot highlighted a spike around 11 a.m.—a potential mystery to dig into.
Silica Concentration Fluctuations: Another plot showed several peaks throughout the day, with 5 a.m., 11 a.m., and 6 p.m. standing out as potential areas for further exploration.
Flotation Column Levels: A sudden change at 3 p.m. caught my attention, prompting questions about operational shifts.

These are some potential feedback ideas to return to the boss. Through these visuals, I learned there are some interesting peaks and dips, but only because these charts are heavily zoomed in on the y-axis. This is done to see the changes but as the analyst you have to be smarter than the graph and realize you have to take into account this zoomed-in scale and compare it to reality. Remember the correlation matrix I mentioned before? It proved there is very little relationship between these variables.

What I Took Away From This Experience
This project was more than a learning opportunity; it was a masterclass in problem-solving. Cleaning messy data, uncovering trends, and using Python to navigate challenges showed me the power of thorough analysis.

I was especially struck by how the % Iron Concentrate fluctuated throughout the day and its relationship with other variables. One would think this naturally but taking another look at all the scales of the axes, everything is relatively stable with minimal fluctuations. The y-axis on every graph is increased by tiny increments. Nothing is shown truly to scale with 0 being the bottom and 100 or the highest possible outcome being shown at the top of the y-axis. It is crucial to take the scale of the charts into account when conducting analysis. All the peaks and dips look intense but they are not when you take into account the scale at which it's being presented. It's like a 10x zoomed-in snapshot of the data and not so much a big picture of the whole horizon. 

Python, which once seemed intimidating, turned out to be an incredibly intuitive tool. I was fairly easy to work with and I look forward to using it more and discovering new uses for it!

### Final Thoughts
Diving into this project transformed the way I see data analysis. Each challenge became an opportunity to grow, and Python cemented itself as a tool I’ll lean on in future endeavors. What began as a curious exploration turned into a passion for analyzing data and understanding how it can influence industries far beyond mining.

### Let’s Connect!
If this story resonated with you or sparked your curiosity, let’s keep the conversation going! Whether you’re interested in mining, data analysis, or are looking for someone to join your team, I’d love to connect on LinkedIn. Don’t hesitate to share your thoughts or ask questions—I’m all ears!
