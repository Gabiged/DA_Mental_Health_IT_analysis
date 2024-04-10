# DA_Mental_Health_IT_analysis
### Mental Health in the Tech Industry
Requirements:<br>
* Perform exploratory data analysis. This should include creating statistical summaries and charts, testing for anomalies, checking for correlations and other relations between variables, and other EDA elements.
* Provide clear explanations in your notebook. Your explanations should inform the reader what you are trying to achieve, what results did you get, and what these results mean.
* Provide suggestions about how your analysis can be improved.
- This data is from Open Source Mental Illness (OSMI) using survey data from years 2014, 2016, 2017, 2018 and 2019. 
- the dataset can be dowloaded: https://www.kaggle.com/datasets/anth7310/mental-health-in-the-tech-industry
- Each survey measures and attitudes towards mental health and frequency of mental health disorders in the tech workplace.
- The survey is conducted online at the OSMI website and the OSMI team intends to use these data to help drive awareness and improve conditions for individuals with mental illness in the IT workplace. 
- It should be noted that as this is an online survey, it may be prone to voluntary response bias and may cause over representation of data. 
- The sample of respondents was not obtained through any random sampling approach. Furthermore, as this is an observational study with potential sampling biases present, causality can not be inferred.
- The results of the survey may not be generalizable to the entire population of Tech/IT workers due to the lack of random sampling. Keeping the above limitations in mind and being cautious with our interpretations, we can still use the data to gain some insight into the state of mental health in the tech workplace.
**To assess mental health support in the workplace, I chose the following features to analyze:**
- the open discussion in the workplace about mental health, and anonymity,
- the impact of the gender distribution of employees,
- Does size of the company relate to an employer formally discussing mental health.
** Used libraries: sqlite3, pandas, seaborn, numpy, matplotlib.
dataset shema:

![Screenshot 2023-03-17 123905](https://user-images.githubusercontent.com/113060033/226151604-499430ed-b16d-412e-a345-05cd2a681f48.png)

* The dataset consists of 3 tables (Answer, Question, Survey).
* The Surveys conducted in 2014-2019, but 2015 year was not surveyed.
* There are 118 questions in the question table in total, but not all questions where asked (2014 - 103 questions; 2016 - 118     questions, 2017-2019 were only 89 questions asked).
* The Answer table contains 236898 rows. There are a total of 4218 respondents in this dataset. The number of respondents varies: 2014 year - 1260 respondents, 2016 year-1433 respondents, 2017 year-756 respondents, 2018 year-417 respondents and 2019 year-352 respondents.
* There are no missing values in the dataset, but attention should be paid to incorrectly (erroneously?) reported data. As an example, the geographical distribution of respondents: 4 respondents indicated "-1" and "other" as their country.  This does not distort the overall question of which country had the highest number of respondents (USA - 2604 respondents).  Hence, this is a biased sample as no equivalent sample was selected. Please note that this is an online survey, so it may be subject to voluntary response bias. The sample of respondents was not randomly selected.

The total amount of information covered by the survey ranges from 2014 to 2019.
It is an online survey with a sufficiently clear geographical dependency, so it cannot be classified as a random survey. However, the nature of the questions available and the number of respondents, 4218, give a good overall picture.
This work is aimed at employees of working age, whether they work for the company or are self-employed, we can see that the most popular age group is between 20 and 40 years old.
The majority of the respondents are male, but the average age for the three gender groups makes it possible to choose not the gender, but the choice of employees as a group.
The data show that only in 2016 the clear answers show an almost equal number of workers with and without a mental disorder diagnosis. However, in the following years, even during the anonymous survey, the respondents were not inclined to give a clear answer to this question.
This leads to the next question of whether the employee is granted anonymity if he chooses the treatment options offered by the employer. To which the overwhelming majority in all years replied that they are not guaranteed anonymity if the employer offers the solution, because in this case the employee is not sure how the employer will react to the mental disorder.
Looking at the extent to which the size of the company affects the employer's concern for their employees through open discussions, we clearly notice that the general trend is negative, but looking at the positive responses, we can make general observation showinge that the higher the number of employees in a company, the more positive the employees' attitude towards the employer's efforts to communicate openly about the employees' mental condition.
How can the company improve its performance so that employees get the psychological help they need, if, as the data show, employees do not express a high level of confidence in the company's discretion. In this case, the survey shows that employees are simply reluctant to discuss or question this type of communication about their psychological issue with other co-workers. The survey shows that employees are willing to discuss it with their supervisors rather all team. This could show trust in the company's leaders.
The survey showed that it would be worthwhile for companies to concentrate on training their leaders and managers to recognize and provide the necessary support to their subordinates. Such a concentration would be more commercially viable than investing in generic discussions or initiatives which, as the results show, do not have the desired effect.
