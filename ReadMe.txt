Requirement: Python 3.7 as minimum

Files:
MLS - python file/script with which performs the required calculations
Report.txt - short file which explains the steps taken to solve the tasks 
Images are provided in the folder to answer some of the task.


Task 1. Which team won the league in Season 1?
The winner in Season 1 is Miami with 138 points.

Task 2.At what point in the season did that team secure their league title?
Miami secure the title in Gameweek 50 in Season 1

Task 3. What result was the biggest upset?
The biggest upset is the draw between Miami and Milwaukee which is evident from the odds of 23.35 for a draw and the rank difference at the end of the season where the two teams are separated by 25 places (right top corner in Fig.1)

    Gameweek           Home       Away  ...  AwayScore   ODDS  RANK_DIFFERENCE
54        12          Miami  Milwaukee  ...          3  23.35               25
50        28          Miami    Atlanta  ...          1  20.52               19
68        52      Arlington    Houston  ...          1  17.44                8
10         2  San Francisco     Boston  ...          1  13.01               18
72        38     New York S  San Diego  ...          2  12.72               21

[5 rows x 7 columns]

Task 4: There are many methods that can be used for predicting the outcomes of football matches. Choose and implement one, and use it to generate predictions for the forthcoming season. Consider how you might test this model, bearing in mind you have results available for the second season.


Start Random Forests Model Building...

Building model with features: Most recent ranking, Average goals scored per game, Average goals conceded per game, Recent form (points from last 5 matches) and Points difference to the next closest position in the league table  

Model building finished

Cross Validation Model Building and Testing in progress...

Cross Validation Finished

Test Set Classification report:

              precision    recall  f1-score   support

     HomeWin       0.55      0.62      0.59       249
        Draw       0.19      0.08      0.11       138
     AwayWin       0.66      0.75      0.71       355

    accuracy                           0.58       742
   macro avg       0.47      0.49      0.47       742
weighted avg       0.54      0.58      0.56       742


Training Set Accuracy: 1.0
Average Accuracy of Cross Validation models: 0.5033
Validation Set Accuracy: 0.6607
Test Set Accuracy: 0.5849
Model performance: model is not optimized and it is currently overfitting.

Task 5 Produce a visualisation showing how likely you predict each team is to finish in each position.

Starting a Monte Carlo Simulation to obtain the probabilities for the end of year standings for each team...

Monte Carlo Simulation Completed


Task 6. Explore the data to your heart’s content


Searching for anomalies in the matches of season 2...
