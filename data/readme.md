# Overview
Models are ranked by their weight and correlation within Numerai's meta-model. The meta-model is an ensemble of all our
data scientist's predictions. Generally, a lower logloss score results in a better rank.

You retain all intellectual property rights to your model. You never have to tell anyone how you built it and you never
have to tell us who you are. You only upload your predictions.

# Datasets
numerai_training_data.csv

Use this dataset to train your machine learning algorithm. The first 21 columns (feature1 - feature21) are features, and
target is the binary class you’re trying to predict.

numerai_tournament_data.csv

Once you’ve built your model, you can use it to generate probability estimates on this new dataset.

# Uploading predictions
To upload your predictions, login and click the Upload Predictions button on the leaderboard. The format of your
prediction upload should be a CSV file with two columns:t_id and probability. The probability column is the probability
estimated by your model of the observation being of class 1.

# The leaderboard and earnings
The public leaderboard displayed on the homepage is calculated on a subset of the total tournament data. Earnings are
calculated on the remainder of the tournament data: the private leaderboard. This discourages overfitting to the public
leaderboard.

Earnings accrue based on the meta-model rank on the private leaderboard. They are presented based on the public
leaderboard rank, but accrue based on the private leaderboard rank.

Earnings are denominated in USD but paid out in bitcoin.


https://numer.ai/rules