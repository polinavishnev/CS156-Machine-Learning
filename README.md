# CS156-Machine-Learning
A collection of substantial projects I completed for the CS156 Machine Learning course. In this course, students were free to choose the topic of each project, as long as it covered one of the models taught in class. I chose to explore the following:

## Project 1: Running Speed Predictor 🏃‍♀️
* Explored the relationship between running data and next day's mean speed using rolling windows (past day, week, or two weeks).
* Dataset: Approximately 600 days of running records with 5 features: distance, duration, step count, max speed, and calories burned.
* Models: Backward stepwise linear regression and random forest regression.
* Best Performing Model: Backward stepwise linear regression using data from one day before.
* Achieved an adjusted-R-squared of 0.50 and a mean-squared error of 0.37 kmph.

## Project 2: Wishlist Clothing Cluster and Aggregator 🛍️
* Clustered and aggregated similar clothing items from my Instagram saved collections based on the Fashion-MNIST dataset and image-processing.
* Training dataset for SVM: Fashion-MNIST dataset with 60,000 images of 10 different clothing items.
* My dataset: 140 pre-processed images of clothes from my Instagram saved collections.
* Models: Hierarchical clustering, k-means clustering, and support vector machine.
* Best Performing Model: Visually, given the unsupervised learning, the hierarchical clustering with 15 clusters performed best.
* Achieved a Ward linkage distance of 31 for the hierarchical clustering. Upon aggregating the clusters (taking the average of the pixels in that cluster), considering that no individual cluster contained only shirts, the accuracy is difficult to measure. Moreover, the SVM model trained on the Fashion-MNIST dataset classified every aggregation as a shirt.

## Project 3: SMA(R)T Goal Classifier with Feedback ✅
* Trained basic classifiers (Logistic Regression, Support Vector Classifier, and Random Forest Classifier) to classify tokenized goals into Specific, Measurable, Action-oriented, and Time-bound categories. Then, combined the three into an ensemble model. Added GPT-2 transformer to suggest next steps to make the goal more S., M., A., or T.
* Dataset: Self-labeled portion of the Kaggle's 2015 New Year's resolutions tweets and Chat-GPT generated goals lacking the SMART characteristics (284 goals in total).
* Models: Logistic Regression, Support Vector Classifier, Random Forest Classifier, Ensemble Voting Classifier, GPT-2 transformer.
* Best Performing Model: The Ensemble Voting Classifier using the soft voting function.
* Achieved an average accuracy score of approximately 83%.
* Note: The relevancy of a SMART Goal is not considered given the need for additional context from the user.

You can check out the extension of this project in the [SMAT Goal Telegram Bot](https://github.com/polinavishnev/SMAT-Goal-Telegram-Bot)! There, I transformed the Jupyter notebook classifier into a Telegram bot that reads the user's input and classifies it into different SMAT goal components. The bot also provides feedback on the user's input and suggests ways to improve it. 