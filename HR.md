<img src="HR_visuals/Title_image.png?raw=true"/>

## Employee Attrition: A Data-Driven Journey

There’s something fascinating about numbers. They tell stories, reveal patterns, and sometimes even surprise us. One moment that really stuck with me during my recent project was when I discovered that younger employees were leaving their jobs more frequently than their older counterparts. This was a twist I didn’t expect, especially given the common belief that companies tend to favor younger employees for their adaptability to new technologies. But as I delved deeper into this analysis, I realized there was so much more to explore about employee attrition.

### Why THIS Project?
My love for statistics inspired me to embark on this project. I’ve always enjoyed digging into data to uncover stories hidden in the numbers. When my HR department boss asked me to analyze employee attrition stats, I jumped at the chance. This project was unique—it wasn’t just about numbers; it was about understanding the people behind those numbers and what might influence their decisions to stay or leave the company.

### What Readers Will Gain
In this article, you’ll learn about employee attrition trends based on my analysis. You’ll discover surprising insights about age, income, and what those might mean for businesses. I’ll share key findings, explain the analysis process, and highlight how data can help us make better decisions regarding employee retention.

### Key Takeaways
Younger employees tend to leave more often than older employees.
There is a weak correlation between age and monthly income.
A linear regression analysis shows that age can explain about 25% of the variance in monthly income.

### Dataset Details
The data I used came from [Kaggle](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset), which is a fantastic resource for datasets. It included information on 1,470 employees, featuring 35 variables like age, attrition status, monthly income, and yearly income. This dataset was perfect for my project because it provided a comprehensive view of employee demographics and behaviors.

I feel it is important to note that this dataset was not clear in defining how the employees left the company. Did they quit on their own or were they laid off? The answer is unknown and is left to your discretion. I feel it makes the most sense that people left voluntarily but it is possible that people were fired or laid off.

### Analysis Process
My analysis journey began with data cleaning and preparation. I then created visualizations to explore relationships within the data. One of the first steps was generating a correlation matrix. Interestingly, while it showed the strongest correlation between monthly income and total working years (0.7729), it confirmed that most relationships were weak. This left me with many questions and a curiosity to dig deeper.

For instance, I created scatterplots to visualize age against monthly income. Seeing younger employees earning more than some older ones was a refreshing surprise. However, when it came to analyzing attrition by age, I used a boxplot and a Welch Two Sample t-test, which revealed a statistically significant difference between the ages of employees who left and those who stayed.

### Visuals and Insights

Correlation Matrix
<img src="HR_visuals/corr_matrix.png?raw=true"/>

The highest value was 0.7729 showing the correlation between monthly income and total working years. This logically makes sense because typically the longer you work somewhere the more money you will make. Most of the other values in the matrix were 0.3 or less indicating a weak relationship. Sadly, this matrix really leaves us with more questions to be asked then revealing any helpful insights.

Scatterplots 
<img src="HR_visuals/Scatterplot_matrix.png?raw=true"/>

When I first saw this, I had trouble understanding how to read it. The boxes with the text indicate the written variable for both that row and column that it is displayed in. The first and rather obvious trend you should see is the positive relationship between age and total working years (see the middle four boxes). I was surprised to see age and monthly income scattered all over the place. It was nice to see some younger employees making more money than some older ones.

Hypothesis Testing and Age Distribution Boxplot 
<img src="HR_visuals/boxplot.png?raw=true"/>

The boxplot comparing the age of those who left versus those who stayed was revealing. I was thrilled to find a statistically significant difference, which confirmed my hypothesis that younger employees are more likely to leave. This insight can help HR teams target retention strategies better.

The boss was curious to see if age was the main reason for people leaving their jobs. So, I made a boxplot to show the age distribution of those who left and those who stayed. They look similar but you can see the median for the "Yes" is lower than the "No." This leads us to the hypothesis that we want to test. Was age the main reason people left?

In R, I tested this what's called a Welch Two Sample t-test. Basically, we have one sample that did leave, and one sample that did stay. I compared the average ages of these two samples and calculate a p-value.

<img src="HR_visuals/t_test.png?raw=true"/>

Because p is less than 0.05, there is a statistically significant difference between the two samples. Those who left were younger than those who stayed! We can see that in the mean comparison at the bottom. Note that x is the first array we passed in and y is the second array we passed in. That is also confirmed in the confidence interval, since both those numbers listed below are negative, we know that the first array is smaller than the second, with confidence.

Linear Regression 

<img src="HR_visuals/linear_regression.png?raw=true"/>

The linear regression analysis showed that age could explain about 25% of the variance in monthly income. This explained quite a bit about income trends, but it also left me curious about what other factors might contribute to attrition.

### Main Takeaways
My findings suggest that age plays a significant role in employee attrition. Younger employees are more likely to leave their jobs, challenging the conventional wisdom that older employees are less adaptable or valuable. This might indicate that younger employees seek more than just a paycheck; they may prioritize factors like company culture and benefits. This data would suggest that older workers value loyalty and stability more and could explain why they stay with their current employer longer. In my experience, attractive employee benefits have always motivated me to stay with an employer, and this is a common trend that companies should not overlook.

### Conclusion and Personal Reflections
This project has taught me a lot about the intricate relationships between employee characteristics and their job satisfaction. The biggest challenge was navigating the data and ensuring I interpreted the results accurately. Through this experience, I’ve gained a deeper appreciation for how data can inform HR practices and improve employee retention.

I hope readers get more curious about statistics. This information can be of great use to other companies and learning what keeps their employees motivated to stay with the company. I would argue that a large part of one's motivation to stay with a company is the benefits offered to them. Great employee benefits are a huge motivator for me when it comes to staying with an employer. I know many others greatly consider this also when they pick their employer.

I hope this exploration inspires you to look more closely at the stories behind the numbers in your own work. If you’re curious about how to apply these insights, let’s connect!

### Call To Action
If you found this analysis engaging, I’d love to hear your thoughts! Connect with me on [LinkedIn](https://www.linkedin.com/in/smsilvey/), and if you or someone you know is looking to hire a data analyst, let’s chat! Feel free to leave a comment with your questions or insights.

[<img src="images/Button.jpg?raw=true"/>](/index.md)
