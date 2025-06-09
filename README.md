# Machine Learning and Tic-Tac-Toe

This project is meant to demonstrate how machine learning can be used to analyze the game of tic-tac-toe and determine the optimal moves to achieve the best outcome possible in a given game. The dataset used provided every possible outcome and board position. In processing this data, we found that we needed a model that could handle the non-binary outcomes of the game (Win/Loss/Tie). 


### Methodology
To prepare the data, we utilized a PySpark SQL database to hold the data that we would use for training and testing of the model. Initially, we used the RandomForest model for our dataset. This gave adequate accuracy for Win or Loss conditions, but did not account for Tie outcomes. From here, we further cleaned the data and changed models to decision tree. Additionally, we increased the depth of the decision tree from 10 to 20 to account for a larger set of possible game outcomes.


### Reference for data source
The data used was sourced from: https://www.kaggle.com/datasets/anthonytherrien/tic-tac-toe-game-dataset
