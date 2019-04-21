# NLP-Sentiment-Analysis
Train a Multilayer Perceptron to predict sentiment score . Using unigram features as input, call the training and testing functions for the Multilayer Perceptron from the tool. 
Q3.1
------Packages and functions------

Import all the packages needed and define all the functions in this part.
convert function to convert the string to vector of word counts.
cross_validation function to split train_data and train_labels into k parts.
cv_modeling function perform multi-perceptron classifier on dataset with k_folds.

------Data Preprocessing------

List all the postive and negative files and read them into: train and train_labels. (Remove punctuations and multiples spaces)

Create a lexicon of all the train file including all the top 10000 frequency words without stopwords. (9855 words remained)

Convert the train reviews into vectors of 9855 dimensions and the value is word count in corresponding review.

------Modeling Part------
Use crossvalidation function to split train data and train labels in to 10 corresponding folds.

Create a grid search dictionary to store the model results.

Run cv_modeling on the processed data and return the accuracy of each model.

----------------------------------------------

Q3.2 

Bulid up model_1 with the tuned hyper parameters and train the model on the whole training set. Return the accuracy.

----------------------------------------------

Q3.3

------Packages and functions------

Import all the packages needed and define all the functions in this part.

Function to generate word2vec representation of the reviews. Stopwords are removed in this function.

***Need to run the ------Packages and functions------ part in Q3.1 if restart python.***

------Data Processing------

Read files first if restart python.

Unzip the google word2vec under the working directory and read it to a dict word2vec.

Convert the review files into vectors using word2vec and the function word2vec_embedding.

------Modeling Part------

Use crossvalidation function to split train vectors and train labels in to 10 corresponding folds.

Create a grid search for tunning parameters.

Run cv_modeling on the processed data and return the accuracy of each model.

------train model on the whole training data------

Bulid up model_2 with the tuned hyper parameters and train the model on the whole training set. Return the accuracy.

----------------------------------------------

Q3.4

------generate new feature------

Generate a new feature: normalized word count(length of each review)

Add the new feature to the train_vector.

------Modeling part------

Train model_3 on the whole training set using the parameter tunned on Q3.3. Return the accuracy.


Q3.5

***Need to run the ------Packages and functions------ part in Q3.1 if restart python.***

------Model Preparation------
Run this part to get trained model_1 with 3 epochs

------Data Processing------

Input test files and convert it into vector of word count representation.

------Model Prediction------
Use model_1 to predict the result of test set and output the classification result.


