<img src="Bank_Vissuals/The-world-bank-7c51155a361e1efba7c704d19b6a5aca.png?raw=true"/>

# Your Tax Dollars Hard at Work

I have always had a strong fascination with money and numbers ever since I was a kid. I remember walking down the toy isle at the store and asking my mom I could have this nerf gun toy. She told me I had to work hard and save my money for it. Meanwhile, I see another kid and his mom grabbing a cool toy and throwing it in their cart. I wondered how they had the money for it in my head. Ever since then I was hooked and wanted money all the time! I was 5 years old.

Fastforward nearly 30 years and here I am with the same curiosity and desire for money. Recently, I was assigned to analyze data from the World Bank. It got me thinking, "where does the world get its money?" Taxes from the governement has to sum it up mostly. We all pay taxes to the government for nearly everything that has a hold of money. Too much if you ask me. So where and who gets all this money? I needed to know and dove into the data.

## Why THIS Project?
I think transpearency is key to see where the money is going and how it is being used. Datasets like this are key to open and honest communication about money transfers/loans. It is crucial to see how much debt nations have to see how much financial burden they have. Too much debt for a country has negative consequences. They appear weak to other countries and less desirable to get future loans for projects from the government.

I wanted answers to these questions:

1. Which countries have the most debt due to the IDA?
2. Which countries paid back their loans the most?
3. What were a few top projects that got the most funding?

## Bottom Line Up Front
The data gave me the following answer to my questions above.

1. India, Bangladesh, and Pakistan are the top three with the most due to the IDA.
2. Interestingly enough, the same top three countries with the most due have also repaided the most back to the IDA.
3. India cracked the top 10 projects twice with 2 COVID-19 related projects. It appears that the top funded project was the **"PEACE in Ukraine Project"** with $4,800,000,000. That's **$4.8 Billion**. That is a lot of tax payer money!

## Data Source
Link to data

"The International Development Association (IDA) credits are public and publicly guaranteed debt extended by the World Bank Group. IDA provides development credits, grants and guarantees to its recipient member countries / economies to help meet their development needs. Credits from IDA are at concessional rates. Data are in U.S. dollars calculated using historical rates. This dataset contains historical snapshots of the IDA Statement of Credits and Grants including the latest available snapshot. The World Bank complies with all sanctions applicable to World Bank transactions" (World Bank's Website).

This basically says that all the money going to these projects in the data are debt and will need to be paid back at some point. The data is labeled current as of Dec. 31, 2024 so it is current and relevant data. It contains almost **70k columns and over 1.3M rows!**

## Data Analysis
To begin, I cleaned what I could from the data to remove any irrelevant information. I was strictly searching for the data to answer my three key questions above.

1. India, Bangledesh, and Pakistan have the most debt due to the IDA from projects. This can be explained due to them having the most projects.

   <img src="Bank_Vissuals/queryanswer1.jpg?raw=true"/>

   <img src="Bank_Vissuals/resultanswer1.jpg?raw=true"/>

I used the SUM function to total to total all the debts from projects and have them categorized by country.



2. I wanted to see which countries were the most finacially responsible in terms of paying back their debts. I was not expecting to see the same top three countries again! India, Bangladesh, and Pakistan have the highest amount repaid to the IDA.

<img src="Bank_Vissuals/queryanswer2.jpg?raw=true"/>

<img src="Bank_Vissuals/resultanswer2.jpg?raw=true"/>

Interesting to see a couple of changes from this top twn chart compared to the first one. Seems like some countries are more eager to pay off their debts than others.


3. Ukraine got the top spot for most expensive project. Kind of makes sense since the whole Russia Ukraine conflict thats been going on for some time now. Then we see India on the top 10 list twice with two COVID related projects.

<img src="Bank_Vissuals/queryanswer3.jpg?raw=true"/>

<img src="Bank_Vissuals/resultanswer3.jpg?raw=true"/>

Kenya made the the top 10 with 3 most expensive projects. Note that they are not in top 10 when it comes to repaying IDA.

## Main Takeaways and Conclusion
Debt is a dual edge sword. It can help you if used smartly and it can destroy you if you let it get out of control. My analysis proves if countries are responsible in taking out loans for projects and can pay them back promptly, then the World Bank is happy to do repeat bsuiness with them. Banks are in business to make money and they do that by issuing out loans. Most of this money comes from all of us paying our taxes so we should all have somewhat of an interest and say in where it gets spent.

SQL is a very powerful tool to analyze large datasets. I can't wait to learn more tricks and tips within SQL. I love how you can pin point very specific peices of data and sort them in a meaningful way. 

## Call to Action
If you enjoyed this article or found it interesting, i encourage you to connect with me on [LinkedIn](www.linkedin.com/in/smsilvey). Also, if you know of anyone who is hiring a data analyst, let's talk. I would like to hear your thoughts on my analysis or any questions you may have.

