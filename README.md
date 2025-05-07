# Nuclear Power Plant Anomaly Detection System

![Nuclear Power Plant](https://www.mdpi.com/electronics/electronics-13-04428/article_deploy/html/images/electronics-13-04428-g001.png)

## Overview

This project implements machine learning models to detect anomalies in nuclear power plant operational data. Early detection of anomalies is critical for preventing accidents and ensuring the safe operation of nuclear facilities.

The system analyzes various sensor readings and operational parameters to identify potential anomalies, helping plant operators take preventive actions before critical failures occur.

## Dataset

The dataset (`Nuclear_Power_Plant_CPS_Dataset.csv`) contains operational data from a nuclear power plant with the following features:

- Reactor Temperature (°C)
- Coolant Flow Rate (L/s)
- Pressure (MPa)
- Radiation Level (μSv/h)
- Turbine Speed (RPM)
- Pump Status (categorical)
- Control Rod Position (%)
- And other operational parameters
- Target variable: Anomaly Detected (Yes/No)

## Features

- **Data Preprocessing**: Handling missing values, encoding categorical variables, and scaling numerical features
- **Class Imbalance Handling**: Using SMOTE (Synthetic Minority Over-sampling Technique) to address imbalanced data
- **Multiple ML Models**:
  - Logistic Regression
  - Random Forest Classifier
  - XGBoost Classifier
  - Support Vector Machine (SVM)
  - k-Nearest Neighbors (KNN)
- **Comprehensive Evaluation**: Accuracy, precision, recall, F1-score, ROC-AUC, and confusion matrices
- **Visualizations**: Performance comparison, ROC curves, feature importance plots

## Getting Started

### Prerequisites

```bash
pip install -r requirements.txt
```

### Running the Analysis

1. Clone this repository
2. Ensure the dataset is in the `/archive` directory
3. Open and run the Jupyter notebook:

```bash
jupyter notebook nuclear_anomaly_detection.ipynb
```

## Project Structure

```
Nuclear-anomaly-detection-system/
├── README.md                         # This file
├── nuclear_anomaly_detection.ipynb   # Main Jupyter notebook with all code and analysis
├── archive/                          # Data directory
│   └── Nuclear_Power_Plant_CPS_Dataset.csv  # Dataset
└── requirements.txt                  # Python dependencies
```

## Models and Results

The notebook compares multiple machine learning models for anomaly detection:

| Model                 | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|-----------------------|----------|-----------|--------|----------|---------|
| Logistic Regression   | TBD      | TBD       | TBD    | TBD      | TBD     |
| Random Forest         | TBD      | TBD       | TBD    | TBD      | TBD     |
| XGBoost               | TBD      | TBD       | TBD    | TBD      | TBD     |
| SVM                   | TBD      | TBD       | TBD    | TBD      | TBD     |
| KNN                   | TBD      | TBD       | TBD    | TBD      | TBD     |

*The table will be filled with actual values after running the notebook*

## Key Visualizations

The notebook generates several visualizations to help understand the data and model performance:
- Confusion matrices for each model
- ROC curves comparing all models
- Feature importance for tree-based models
- Performance metrics comparison

## Future Improvements

- Hyperparameter tuning to optimize model performance
- Deep learning approaches (LSTM, Autoencoders)
- Time series anomaly detection techniques
- Ensemble methods combining multiple models
- Feature engineering to create more predictive variables

## References

- [Anomaly Detection and Analysis in Nuclear Power Plants](https://www.mdpi.com/3038026)
- SMOTE: [Synthetic Minority Over-sampling Technique](https://arxiv.org/abs/1106.1813)

## License

This project is licensed under the MIT License - see the LICENSE file for details.

