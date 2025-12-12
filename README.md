# Chicago Car Crashes Prediction

<div align="center">
  <img src="chicago-car-crashes.webp" alt="Chicago Car Crashes Prediction" width="600"/>
</div>

Car accidents is an important and directly related topic in people's daily lives, According to statistics from the Illinois Department of Transportation (IDOT), there were 92,092 car accidents in the city of Chicago in 2020. Of these, 133 accidents resulted in fatalities and 19,755 caused injuries and 12,526 involved visible injuries that did not incapacitate the victim. Machine learning can be a useful tool for analyzing and reducing the risk of crashes. in this project, an analysis of Chicago traffic accident data of year 2020 is demonstraed, followed by prediction of accident primary causes based on random forest model.

## Data Collection

Chicago car crashes data can be obtained from the [Chicago Data Portal](https://data.cityofchicago.org/).

The links and descriptions of datasets are listed below:

-   **[Traffic Crashes - Crashes](https://data.cityofchicago.org/Transportation/Traffic-Crashes-Crashes/85ca-t3if)** - Main crash dataset containing crash records, locations, dates, and primary contributory causes
-   **[Traffic Crashes - Vehicles](https://data.cityofchicago.org/Transportation/Traffic-Crashes-Vehicles/68nd-jvt3)** - Vehicle information including vehicle type, make, model, and vehicle-related contributory factors
-   **[Traffic Crashes - People](https://data.cityofchicago.org/Transportation/Traffic-Crashes-People/u6pd-qa9d)** - Information about people involved in crashes including age, sex, and injury severity

For detailed column descriptions, see [Columns Description.md](Columns%20Description.md).

## Goal

Create a model to predict and classify prime contributory factors of car crashes related to year 2020.

## Metrics

The following evaluation metrics are used to assess model performance:

-   **accuracy_score** - Measures the overall correctness of predictions, calculated as the ratio of correct predictions to total predictions
-   **roc_auc_score** - Area Under the Receiver Operating Characteristic Curve, which evaluates the model's ability to distinguish between classes, particularly useful for imbalanced datasets

## Models - Classifiers

This project implements and compares multiple machine learning classifiers:

-   **Decision Tree Classifier** - A tree-based model that makes decisions by splitting data based on feature values, providing interpretable results
-   **Random Forest Classifier** - An ensemble method that combines multiple decision trees to improve prediction accuracy and reduce overfitting
-   **Bagging Classifier** - Bootstrap aggregating classifier that trains multiple models on different subsets of data and combines their predictions

## Library / API

The following libraries and APIs are used in this project:

-   **Python** version 3.8.5 - Programming language
-   **Pandas** - Data manipulation and analysis library for handling structured data
-   **Seaborn** - Statistical data visualization library built on matplotlib
-   **Matplotlib** - Comprehensive plotting library for creating static, animated, and interactive visualizations
-   **NumPy** - Fundamental package for scientific computing with Python, providing support for large multi-dimensional arrays
-   **Scikit-learn** - Machine learning library providing various classification, regression, and clustering algorithms

## Conclusion

The Random Forest Model successfully predicts car crashes with **78% accuracy**, demonstrating strong performance even when dealing with an imbalanced dataset containing 102 features. The model effectively identifies primary contributory factors of car crashes, providing valuable insights for traffic safety analysis.

### Key Achievements

-   Achieved 78% accuracy with imbalanced data
-   Successfully handled 102 features
-   Identified primary contributory causes of crashes
-   Demonstrated practical applicability for real-world scenarios

### Future Improvements

The accuracy of the model can be further improved by:

-   Including data from previous years (2015-2020) to capture temporal patterns and trends
-   Implementing advanced feature engineering techniques
-   Exploring ensemble methods combining multiple models
-   Applying techniques specifically designed for imbalanced datasets

### Use Cases

As a potential use case, the developed model can be used as a **car accidents prediction system** to predict car crash occurrences in real-time, enabling:

-   Proactive traffic management and safety measures
-   Identification of high-risk areas and times
-   Data-driven decision making for urban planning
-   Enhanced public safety initiatives
