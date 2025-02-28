<img src="healthcare_visuals/titleimage.jpg?raw=true"/>

# Healthcare Analysis using SQL


February 26, 2025

I’ll never forget the stories my mother shared about her days as a nurse. Amidst the rush and the chaos of a busy hospital, she often spoke about the challenges faced by healthcare professionals. Her passion sparked my curiosity about how data could help streamline operations and improve patient care. I embarked on a journey to analyze ten years' worth of diabetic patient data across 130 hospitals. What I uncovered was both surprising and eye-opening.

### Why THIS Project? 

My motivation for this project stemmed from my admiration for my mother's work. I've always been fascinated by hospital operations, especially how data plays a crucial role in enhancing efficiency. The experiences she shared highlighted the need for better resource allocation in healthcare, which prompted me to explore how patient data could shed light on busy departments and patient demographics.

### What Readers Will Gain

By reading this article, you’ll gain insights into how data analysis can improve hospital efficiency. I’ll share key findings about patient stays, departmental activity, and demographic trends that can inform better resource management in healthcare settings.

### Key Takeaways:

- The average hospital stay for diabetic patients is 4 days.
- Cardiology is the busiest department by patient count.
- Patient visits are fairly evenly distributed across different races.

### Dataset Details 

The dataset I used was sourced from Kaggle and the UCI Machine Learning Repository. It includes over 100,000 records of diabetic patients, compiled over ten years, with more than 50 columns of valuable information. This rich dataset was perfect for uncovering trends and insights about hospital operations.

*The origin of the data can be found [here](https://archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008)*

### Analysis Process

My analysis journey began with cleaning the data, which involved checking for inconsistencies and ensuring the accuracy of the records. I utilized SQL for visualization and analysis, creating graphs that highlighted trends such as patient stays and departmental activity. One surprising finding was the average hospital stay of 4 days, which was much longer than I anticipated. I had expected lab procedures for diabetic patients to be quicker, perhaps 1 to 2 days max.

### Visuals and Insights

<img src="healthcare_visuals/histogram.png?raw=true"/>

Histogram of Patient Counts: This visualization shows how many days patients spent in the hospital, with a peak at 3 days but an average of just over 4 days. This insight suggests that while many patients are discharged quickly, some may require extended stays due to complications. This query used the RPAD function to illustrate a bar chart with stars where each star represents 100 patients.


<img src="healthcare_visuals/INNER_JOIN_health_and_demographics_tables.png?raw=true"/>

INNER JOIN Query Results: Joining the demographics and health data tables allowed me to analyze patient visits by race. The management team wanted to know if there were any correlations between the patient's health data and the patient's race. The primary key that linked the two tables was the patient number as seen above.


<img src="healthcare_visuals/races_equal_treatment.png?raw=true"/>

Any racial bias with treatment?: I was pleased to see an even distribution, indicating no significant racial bias in how often different racial groups had lab procedures done. Management wanted to know the average number of lab procedures grouped by race and ordered from most to least.


<img src="healthcare_visuals/top5_specialties.png?raw=true"/>

Top 5 Hospital Specialties: The analysis also revealed the top 5 specialties with over 50 patients and an average of 2.5 procedures per patient. This information is crucial for hospital leadership, as it highlights areas that may need additional resources or staffing. Although thoracic surgey had the most average procedures done, it had the lowest patient count. Cardiology on the other hand, had the most patients by far with an eye-opening 5352 with an average of 2.7 procedures. Hospital management should focus most of their resources on maintaining and improving their cardiology departments.


<img src="healthcare_visuals/CONCAT_report.png?raw=true"/>

Top 50 Patient Medications Report Summary: 

The boss asked me to write a summary for the top 50 medication patients and break any ties with the number of lab procedures (highest at the top). Hospital management wanted me to come up with a report showing the following: patient number, race, whether or not they were readmitted, their medications, and finally the number of lab procedures done. This report could prove useful in examining hospital expenses for medications and lab procedures and shed some light on their effectiveness.

To show this nicely in SQL, the CONCAT function is needed to combine all the data strings into one column. I had to first change the data type to integer for all the relevant numeric values so SQl would recognize them better using the ALTER function. Then the CASE WHEN function is needed here to show if the patient was ever readmitted to the hospital.

This report interestingly shows that Caucasians had the most medications for their diabetes and more lab procedures were done. Are Caucasians more prone to being diagnosed with diabetes? This data seems to say yes but more study and investigation should be done on this to come up with better insight.

### Main Takeaways

SQL is an incredible tool that can enhance efficiency in healthcare and other industries.
The data analysis indicates that cardiology departments are crucial for patient care, necessitating careful resource management.
Understanding patient demographics and average stays helps hospitals prepare for patient influx and allocate staff accordingly.
Caucasians have the most patient medications for diabetes-related hospital visits.

### Conclusion and Personal Reflections

This project taught me much about the impact of data in healthcare. Specifically, how SQL is so useful in gathering vital information from large datasets. One challenge I faced was ensuring my data analysis was accurate and meaningful. I overcame this by double-checking my work and seeking out new ways to do things in SQL. This experience has impacted my perspective on the importance of data in decision-making, steering me toward a future that incorporates data analysis.

It is very common to combine multiple tables within your database to get more insightful answers to business problems and questions. Knowing the different SQL functions and when to use them is the key to success with SQL and database analysis. I look forward to continuing my SQL knowledge and hope to use its power to help generate positive results for my stakeholders.

I invite you to connect with me to discuss these findings further! Whether you have questions or insights, or want to share your experiences in healthcare data analysis, I’d love to hear from you.
