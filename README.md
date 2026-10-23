# End-to-End ML Model 

Code for Module 2 of the AI & ML course , collected in one Jupyter notebook. It covers two things: a full machine learning project on housing prices, and a classifier for handwritten digits.

## What the notebook covers

Part 1 builds a regression model on the California Housing dataset (1990 census). It goes through:

- downloading and inspecting the data
- splitting off a test set with random, hash-based and stratified sampling
- plotting the data and checking correlations
- cleaning missing values, encoding categories, scaling features and wrapping it all in pipelines
- training Linear Regression, Decision Tree and Random Forest models
- comparing them with cross-validation, tuning with grid search and scoring the final model on the test set

Part 2 works on MNIST. It trains a "5 or not 5" classifier with SGD, then looks at accuracy, the confusion matrix, precision, recall, F1 and the ROC curve. After that it moves to multiclass classification, error analysis, multilabel output and image denoising.

## Running it

Install the libraries:

    pip install numpy pandas matplotlib scipy scikit-learn joblib jupyter

Then open the notebook and run the cells from top to bottom:

    jupyter notebook "End-to-End ML Model(learning).ipynb"

The quotes matter because the file name has spaces and brackets. You can also upload the notebook to Google Colab, which needs no setup.

## Things to know

- The first run needs an internet connection. It downloads the housing data from GitHub and MNIST through scikit-learn.
- A few cells are slow, mainly the grid search and the KNN cell in the multilabel section. Expect about 15 minutes for the whole notebook.
- The original book code dates from 2019, and some of it fails on current libraries. I changed those lines and marked each one with a `# CHANGED` comment.
- Part 1 was run start to finish with scikit-learn 1.8 and pandas 3.0 on Python 3.12. Your scores may differ slightly from the ones printed in the book.

## Credit

The code comes from Chapters 2 and 3 of *Hands-On Machine Learning with Scikit-Learn & TensorFlow* by Aurélien Géron (O'Reilly). The author's own notebooks are at https://github.com/ageron/handson-ml2. This repo is a personal study copy and is not affiliated with the author or publisher.
