## NFL Big Data Bowl

As part of the **Kaggle NFL Big Data Bowl 2020**, I developed a sequential neural network to predict the number of rushing yards an NFL team would gain/lose on each play.

### Data Manipulation

The data provided was part of NFL's NextGen Stats. The training data was broken down play-wise into 22 rows. Each row corresponding to a single player on the field. The data points included fields such as player orientation, positional coordinates on the field, offensive formation, defensive formation, weather conditions, speed, weight, acceleration, etc.
I developed around *30 new features* based on our understanding of the game. A few features I created were **momentum, yards gained vs distance to goal, bucketed jersey numbers**, etc. I used an *ensemble feature importance algorithm* to select a total of **24 features from a total of around 70**.

### Modeling

A TensorFlow based *sequential neural network* was used to generate the final predictions. We optimized our neural network using *Bayesian Hyperparameter tuning techniques* to determine the optimal number of layers, nodes, dropout, etc.

### Results

The testing for this project was unique in that live matches were used to test the predictions. My algorithm was run prior to each match from mid-December to the end of the season. My team finished in the top 30% worldwide on the Kaggle leaderboard, and we were one of the few all-University teams.
