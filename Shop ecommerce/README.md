# Shop Ecommerce ML Project

## Overview

This project analyzes online shopper behavior to predict whether a visitor will generate revenue (make a purchase) using machine learning techniques. The analysis uses the Online Shoppers Intention dataset and implements a Decision Tree Classifier with hyperparameter tuning.

## Dataset

- **File**: `shop_smart_ecommerce.csv`
- **Source**: Online Shoppers Purchasing Intention Dataset (UCI Machine Learning Repository)
- **Description**: Contains various features about website visitors including page views, session duration, visitor type, and whether they made a purchase.

### Column Descriptions

- **Administrative**: Number of pages visited in the Administrative category
- **Administrative_Duration**: Total time spent on Administrative pages (in seconds)
- **Informational**: Number of pages visited in the Informational category
- **Informational_Duration**: Total time spent on Informational pages (in seconds)
- **ProductRelated**: Number of pages visited in the ProductRelated category
- **ProductRelated_Duration**: Total time spent on ProductRelated pages (in seconds)
- **BounceRates**: Percentage of visitors who enter the site from a page and then leave without viewing other pages
- **ExitRates**: Percentage of pageviews on a page that were the last in the session
- **PageValues**: Average value for a web page that a user visited before completing an e-commerce transaction
- **SpecialDay**: Closeness of the site visiting time to a special day (e.g., Mother's Day, Valentine's Day) on a scale of 0 to 1
- **Month**: Month of the visit (e.g., Feb, Mar, etc.)
- **OperatingSystems**: Operating system used by the visitor (categorical)
- **Browser**: Browser used by the visitor (categorical)
- **Region**: Geographic region from which the session originated (categorical)
- **TrafficType**: Traffic source that brought the visitor to the site (categorical)
- **VisitorType**: Type of visitor (New Visitor, Returning Visitor, Other)
- **Weekend**: Boolean indicating whether the visit occurred on a weekend
- **Revenue**: Target variable - whether the visit resulted in a purchase (True/False)


## Requirements

- Python 3.x
- Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn

## Installation

1. Clone the repository
2. Install required packages:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
   ```

## Usage

1. Open the Jupyter notebooks in VS Code or Jupyter Lab
2. Run the cells in order to:
   - Load and explore the data
   - Preprocess features (numerical and categorical)
   - Train Decision Tree model with GridSearchCV
   - Evaluate model performance

## Model

- **Algorithm**: Decision Tree Classifier
- **Preprocessing**: StandardScaler for numerical features, OneHotEncoder for categorical features
- **Hyperparameter Tuning**: GridSearchCV with F1 score optimization
- **Evaluation Metrics**: Classification report, confusion matrix, F1 score

## Model Results

### Best Hyperparameters (from GridSearchCV)

- **criterion**: gini
- **max_depth**: 2
- **min_samples_split**: 2
- **min_samples_leaf**: 5

### Test Set Performance

```
              precision    recall  f1-score   support

           0       0.96      0.88      0.92      2055
           1       0.58      0.81      0.68       411

    accuracy                           0.87      2466
   macro avg       0.77      0.85      0.80      2466
weighted avg       0.90      0.87      0.88      2466
```

**Confusion Matrix (Test Set):**

```
[[1818  237]
 [  80  331]]
```

**F1 Score (Test Set):** 0.676

### Training Set Performance

```
              precision    recall  f1-score   support

           0       0.96      0.89      0.92      8367
           1       0.56      0.81      0.66      1497

    accuracy                           0.87      9864
   macro avg       0.76      0.85      0.79      9864
weighted avg       0.90      0.87      0.88      9864
```

## Summary

The Decision Tree Classifier achieved **87% accuracy** on the test set with strong performance on predicting non-revenue visits (Class 0: 96% precision) while maintaining reasonable recall for revenue-generating visits (Class 1: 81% recall). The F1 score of 0.68 for the minority class (revenue) indicates good balance between precision and recall.

