# Predict-NBA-Game-Outcomes

The purpose of this project was to explore NBA data from https://www.sports-reference.com/ and to build the best classification machine learning model possible on the extracted data. Data was extracted from the 2013-2014 season from the months of October to April as well as from the 2012-2013 season (the ladder for getting the rankings from the previous year). The baseline home win percentage for this season was 56.83% and the goal was to generate a model that would have better returns than this baseline. The feattures that were eventually selected to feed into the models were:

- Whether or not the home team won their last game.
- Whether or not the visiting team won their last game.
- The rankings of each team based on last years ladder. 
- The team name.

Initially the classifier models used were a decision tree and a random forest. They were fed different data at different points along the way but ultimately the data above gave the best general accuracy (evaluated with F1 scores). A bar graph was generated to visualize the performance of these different classifiers with different data. From the visual you can see that the random forest model generated the most generally accurate resutls (according to F1 score).

![Image description](link-to-image)

After that logistic regression, decision tree (with different method), naive bayes, K-nearest neighbors, random forest (with different method), and xgboost classifiers were applied to the data and their general accuracies (not evaluated with F1 score but used accuracy_score method) were evaluated. 
