# Module 2: End-to-End ML Project & Classification

Code for **Module 2** of the AI & ML course (21AI63), written as a Jupyter notebook.

The code follows two chapters of *Hands-On Machine Learning with Scikit-Learn & TensorFlow* by Aurélien Géron:

| Part | Topic | Dataset |
|------|-------|---------|
| 1 | End-to-end machine learning project (regression) | California Housing (1990 census) |
| 2 | Classification | MNIST handwritten digits |

## What's inside

**Part 1: California housing prices**
- Downloading and loading the data, quick data inspection
- Creating a test set (random, ID-hash based, and stratified sampling)
- Exploring and visualizing the data, correlations, attribute combinations
- Data preparation: missing values, categorical encoding, custom transformers, feature scaling, pipelines
- Training and comparing models: Linear Regression, Decision Tree, Random Forest
- Cross-validation, grid search, feature importance, final test-set evaluation

**Part 2: MNIST classification**
- Binary classifier (the "5-detector") with `SGDClassifier`
- Performance measures: cross-validation, confusion matrix, precision, recall, F1, ROC curve
- Multiclass classification (OvA / OvO)
- Error analysis
- Multilabel and multioutput classification

## Files

| File | Description |
|------|-------------|
| `Module-2-code-only.ipynb` | All the code from the module, in order |

## Requirements

- Python 3.9+
- numpy, pandas, matplotlib, scipy, scikit-learn, joblib, jupyter

```bash
pip install numpy pandas matplotlib scipy scikit-learn joblib jupyter
```

## How to run

```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
jupyter notebook Module-2-code-only.ipynb
```

Or open it directly in [Google Colab](https://colab.research.google.com/) (upload the notebook or open it from GitHub). Nothing needs to be installed there.

Run the cells from top to bottom.

## Notes

- An internet connection is needed on the first run to download the housing data and MNIST.
- Some cells are slow (Random Forest, grid search, and the multilabel KNN cell in Part 2). The whole notebook can take around 15 minutes or more.
- The original book code is from 2019. A few lines were updated to work with current scikit-learn and pandas, and each is marked with a `# CHANGED` comment in the notebook.
- Your numbers (RMSE, accuracy, and so on) may differ slightly from the ones printed in the book.

## Credits

Based on Chapters 2 and 3 of *Hands-On Machine Learning with Scikit-Learn & TensorFlow* by Aurélien Géron (O'Reilly). The book's own code and notebooks are at https://github.com/ageron/handson-ml2. This repository is for learning purposes only and is not affiliated with the author or publisher.
