# Machine Predictive Maintenance Classification
### Failure Prediction & Comparative Algorithm Analysis

## 1. Project Overview
This project focuses on predicting machine failures using industrial sensor data (e.g., temperature, torque, and rotational speed). The goal is to evaluate the effectiveness of various machine learning models in identifying potential breakdowns to support automated maintenance decision-making.

## 2. Technical Stack
* **WEKA Platform:** The primary environment used for data mining, model training, and performance evaluation.

## 3. Methodology
The project follows a systematic approach to data preparation and modeling:

### A. Data Preprocessing
To ensure high-quality inputs for the classifiers, the following transformations were implemented:
* **Feature Encoding:** Applied `NominalToBinary` to handle categorical attributes.
* **Data Balancing:** Used the `Resample` technique to address class distribution, ensuring the model remains robust across different failure scenarios.
* **Type Optimization:** Utilized `NumericToNominal` to align attribute types with the requirements of specific classification algorithms.

### B. Modeling & Evaluation
* **Supervised Learning:** A comparative study was conducted across multiple categories, including Tree-based models (J48, Random Forest), Rule-based models (Decision Table), and Ensemble methods (AdaBoostM1).
* **Evaluation Metrics:** Accuracy was used as the primary performance indicator. Additionally, Mean Absolute Error (MAE) was monitored to assess the probability deviation and the confidence level of the predictions.

## 4. Results & Observations
* **Performance:** The **Decision Table** algorithm achieved the highest accuracy of **99.66%**, followed by **J48** and **AdaBoostM1**, both exceeding 99%.
* **Comparison:** Tree-based and rule-based models demonstrated superior performance in capturing non-linear relationships within the sensor data compared to baseline probabilistic models.
