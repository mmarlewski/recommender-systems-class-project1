# recommender systems class project 1

### Project description

This is a completed project 1 from systems recommender class.
We were given two jupyter notebooks with unfinished data preparation and recommender to work with.
Our task was to finish data preparation in first notebook, then prepare user and item features as well as finish the recommender in second notebook.
Our goal was to achieve the best hr@10 score in the final evaluation.
The solution contains two complete jupyter notebooks in ipynb and html formats.

### Required python dependencies

numpy        == 1.20.1
pandas       == 1.2.3
matplotlib   == 3.3.4
seaborn      == 0.11.1
IPython      == 7.21.0
scikit-learn == 0.24.1
hyperopt     == 0.2.7

### Implemented features

For every user from thier reservations:
- number of reservations (interactions)
- one-hot encoding of every feature value
- number of every feature values
- probability distribution of every feature values
- average value for bucket features (buckets were mapped to values)
- most popular value of every feature (each value is represented with a number)

For every item from its features:
- one-hot encoding of every feature value
- min and max value of feature (buckets were mapped to values)

### Final score

The highest hr@10 score I achieved was 0.196271 with one-hot encoded user and item features using LinearRegressionCBUIRecommender with parameters: {'n_neg_per_pos': 6}
