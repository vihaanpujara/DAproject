NBA analysis of Basketball Players Stats per Season - 49 Leagues
Dataset used:
https://www.kaggle.com/jacobbaruch/basketball-players-stats-per-season-49-leagues
BY:
Vihaan Pujara – PES2201800016
Keerthana.V – PES2201800658
Neha Sankad – PES2201800398

We have used Jupyter notebook to work on our dataset.
Libraries used:
pandas, numpy, matplotlib.pyplot, seaborn, matplotlib.gridspec, plotly.graph_objs, plotly.express, make_subplots etc.
Data cleaning: 
First of all the columns having too many missing values or the ones which are not useful for our project are removed, for eg: birth_month, birth_date, highschool. Also those rows are removed which are having more than two missing values. 
Preprocessing: 
The missing values in the numerical columns are replaced by the mean of the entire columns. New columns like FG Conversion Rate, Points Per Game, Overall Performance and 3PA Conversion Rate are created to understand the nature of the dataset in more efficient manner.
Visualizations:
No. of players in different seasons
Leagues presented in dataset
No. of players in different Nationality
Player FGA & FGM Distribution
Top players (max point scored)
Top5 player scores trend
Points Per Game VS Season
Distribution of Age
Season VS Three Points Made (3PM)
Height VS Point/game
Boxplot

ML Modelling:

we have normalised data and found the correlation btw field goals made and the points, and points versus minutes played which resulted in the positive correlation. Firstly, we have considered GP, MIN, FGM, FGA, 3PM and PTS for our model prediction and have split the data into training and test set by 70% and 30% respectively. We have used KNN, Linear SVM, Random Forest Classifier and Gradient tree boosting models for the above dataset. Based on the resits of modelling, KNN and Linear SVM model doesn’t provide the required predictions. We have used the K-means clustering to make 5 clusters based on 3PM, TOV, PF, REB, SAT, STL, BLK, PTS to categorise the players. We have used the Linear regression model to predict the players ratings of the year 2018- 19 by using the previous ratings from the years 1999-2017. The r2 value is 0.986627825370004 and Pearson’s Correlation is 0.99341863830012.

