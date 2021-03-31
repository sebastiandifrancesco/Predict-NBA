# Predict-NBA-Game-Outcomes

The purpose of this project was to explore NBA data from https://www.sports-reference.com/ and to build the best classification machine learning model possible on the extracted data. Data was extracted from the 2013-2014 season from the months of October to April as well as from the 2012-2013 season (the ladder for getting the rankings from the previous year). The baseline home win percentage for this season was 56.83% and the goal was to generate a model that would have better returns than this baseline. The feattures that were eventually selected to feed into the models were:

- Whether or not the home team won their last game.
- Whether or not the visiting team won their last game.
- The rankings of each team based on last years ladder. 
- The team name.

Initially the classifier models used were a decision tree and a random forest. They were fed different data at different points along the way but ultimately the data above gave the best general accuracy (evaluated with F1 scores). A bar graph was generated to visualize the performance of these different classifiers with different data. From the visual you can see that the random forest model generated the most generally accurate results (according to F1 score; 0.6229).

![Image description](https://github.com/sebastiandifrancesco/Predict-NBA-Game-Outcomes/blob/main/decition_tree_random_forest_models.PNG)

After that logistic regression, decision tree (with different method), naive bayes, K-nearest neighbors, random forest (with different method), and xgboost classifiers were applied to the data and their general accuracies (not evaluated with F1 score but used accuracy_score method) were evaluated. The random forest had an accuracy score of 0.9303030303030303.

![Image description](https://github.com/sebastiandifrancesco/Predict-NBA-Game-Outcomes/blob/main/models_OOP_template1.PNG)

Finally I used the tuned random forrest model on the 2018-2019 season gathering all the data in the same way I did for the 2013-2014 season. The baseline for this season was home teams won 58.76% of the time. The tuned random forrest model when applied gave an accuracy of 79.4% (F1 score was 0.79). This needs to be further explored to understand why the accuracy was so much higher than before.

The models after this were created from the 2018-2019 data. The purpose of this is for future use of using the models to predict the current NBA seasons games. Further analysis that could be done would include calculating an expected value (profit) of a sports betting strategy using the models.
