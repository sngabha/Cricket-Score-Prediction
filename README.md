Cricket-Match-Target-and-Winner-Prediction
==========================================

 

In this project, we aim to build a solution using machine learning, 
that can predict the runs scored by team in first innings (target score) 
and also predict the winner of the match.

 

**Directory Structure**


\----Data Preprocessing

\--------Batsmen Profile.ipynb -\> *Contains preprocessing logic to build the profile of batsmen
									from ball by ball raw data. Data extracted: Average run and Balls faced.*

\--------Bowler Profile.ipnyb -\> *Contains preprocessing logic to build the profile of bowlers
								   from ball by ball raw data. Data extracted: Economy and Average no of wickets.*
									
\--------Average Stats.ipnyb -\> *Contains preprocessing logic to calculate average metrics for
								  Batsmen and bowlers.*

\--------Overall Match Stats.ipnyb -\> *Contains preprocessing logic to calculate line up features for 
										a match using the pre-calculated average stats.*

										
\----Derived Stats

\--------batsmen_stats.pkl -\> *Contains batsmen profile information, stored as a pickled dataframe.*

\--------bowlers_stats.pkl -\> *Contains bowler profile information, stored as a pickled dataframe.*

\--------batsmen_average_data.pkl -\> *Contains batsmen profile information, stored as a pickled dataframe.*

\--------bowlers_average_data.pkl -\> *Contains bowler profile information, stored as a pickled dataframe.*

\--------batsmen_stats.pkl -\> *Contains batsmen profile information, stored as a pickled dataframe.*

\--------match_stats_train.pkl -\> *Contains training data formed using pre-calculated stats. Stored 
									as a pickled dataframe.*

\--------match_stats_test.pkl -\> *Contains testing data formed using pre-calculated stats. Stored 
								   as a pickled dataframe.*
 

\----Regression Models

\--------Linear and Polynomial Regression.ipynb -\> *Contains Linear and polynomial regression analysis.*

\--------SV Regression.ipynb -\> *Contains support vector regression analysis.*

\--------Random Tree Regressor.ipynb -\> *Contains Random Tree Regression analysis.*

\--------Gradient Boosted Regression.ipynb -\> *Contains Gradient Boosted Regression analysis.*


\----deliveries.csv -\> *Contains raw data of IPL Matched from year 2008 to 2017. Taken from Kaggle - URL:
						 https://www.kaggle.com/manasgarg/ipl*
						 
						 
\----matches.csv -\> *Contains raw data of IPL Matched from year 2008 to 2017. Taken from Kaggle - URL:
						 https://www.kaggle.com/manasgarg/ipl*
						 

						 
**How to run the Project?**

Please perform the steps in the same order.
 

1.  Run Preprocessing notebooks present in "Data Preprocessing" folder in the
	follwoing order: 'Batsmen Profile.ipynb' -> 'Bowler Profile.ipnyb' ->
	'Average Stats.ipnyb' -> 'Overall Match Stats.ipnyb'. Once these are
	executed all required data for training models will be saved in "Derived Stats"
	folder.

2.  All of the regression analysis can be found in "Regression Models" folder.
	These notebooks can be run in any order to see the model performance.