# AirPredict: AQI Prediction using Classification Algorithms

AirPredict is a machine learning project that leverages classification algorithms to predict the Air Quality Index (AQI) of various cities in India. By analyzing historical AQI data spanning from 2015 to 2020, this model can accurately classify air quality levels and help predict future pollution trends.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Algorithms Used](#algorithms-used)
- [Data](#data)
- [Project Structure](#project-structure)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [How to Run](#how-to-run)
- [Results](#results)
- [Model Performance](#model-performance)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Air pollution is a significant environmental risk to health, and monitoring air quality is essential for both public health and environmental policy. The Air Quality Index (AQI) is a measure used by government agencies to communicate air quality to the public. This project aims to build predictive models that can classify air quality levels based on pollutant concentrations and meteorological factors.

## Features

- 📊 Predicts the AQI based on historical data and pollutant concentrations
- 🏷️ Classifies AQI into categories (Good, Moderate, Unhealthy for Sensitive Groups, Unhealthy, Very Unhealthy, Hazardous)
- 🤖 Supports multiple machine learning classification algorithms
- 📈 Visualization of AQI trends and predictions across cities
- 📋 Comprehensive analysis across 26 Indian cities
- 🎯 High accuracy models with detailed performance metrics

## Algorithms Used

The project explores various machine learning classification algorithms to find the most accurate model for AQI prediction:

- **Logistic Regression** - Linear classification model
- **Decision Trees** - Tree-based classification with feature importance
- **Random Forest** - Ensemble method combining multiple decision trees
- **Support Vector Machines (SVM)** - Powerful kernel-based classifier
- **K-Nearest Neighbors (KNN)** - Instance-based learning algorithm

## Data

The dataset used in this project contains comprehensive historical AQI data from **26 cities across India**, spanning from **2015 to 2020**.

### Cities Included:
Ahmedabad, Delhi, Mumbai, Bengaluru, Chennai, Gurugram, Visakhapatnam, Jaipur, Thiruvananthapuram, Amaravati, Brajrajnagar, Talcher, Kolkata, Guwahati, Coimbatore, Shillong, Chandigarh, Bhopal, Kanpur, Lucknow, Patna, Agra, Varanasi, Indore, Srinagar, Jodhpur

### Data Features:
- PM2.5 and PM10 concentrations
- NO2, SO2, CO levels
- Ozone (O3) concentrations
- Weather parameters (Temperature, Humidity, Wind Speed)
- AQI values and classifications

## Project Structure

```
Air-quality-prediction-ml-algorithms/
├── README.md
├── AirPredict.ipynb          # Main Jupyter notebook with complete analysis
├── data/                      # Dataset files
│   └── aqi_data.csv          # Historical AQI data
└── results/                   # Model outputs and visualizations
    ├── model_comparison.csv
    └── predictions.csv
```

## Prerequisites

- Python 3.7.10 or higher
- Jupyter Notebook
- pip (Python package manager)

## Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/darshan12345678910/Air-quality-prediction-ml-algorithms.git
   cd Air-quality-prediction-ml-algorithms
   ```

2. **Install Dependencies:**
   Ensure you have Python 3.7.10 installed. Then, install the necessary Python packages using pip:
   ```bash
   pip install -r requirements.txt
   ```
   
   Or install packages individually:
   ```bash
   pip install numpy pandas scikit-learn matplotlib seaborn jupyter
   ```

3. **Verify Installation:**
   ```bash
   python --version
   ```

## How to Run

1. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

2. **Open and Run the Notebook:**
   - Navigate to and open `AirPredict.ipynb`
   - Run all cells sequentially (Shift + Enter) or use "Run All" from the Cell menu
   - The notebook will:
     - Load and preprocess the data
     - Train multiple classification models
     - Evaluate model performance
     - Generate visualizations
     - Display predictions for each city

3. **View Results:**
   - Model performance metrics (Accuracy, Precision, Recall, F1-Score)
   - Confusion matrices for each algorithm
   - Feature importance analysis
   - AQI predictions and classifications

## Results

This project demonstrates the effectiveness of various machine learning models in predicting AQI categories. The performance of each model is evaluated based on:

- **Accuracy** - Overall correctness of predictions
- **Precision** - Accuracy of positive predictions
- **Recall** - Ability to identify all positive instances
- **F1-Score** - Harmonic mean of precision and recall

### Key Findings:
- Random Forest generally achieves the highest accuracy for AQI classification
- SVM performs well with proper hyperparameter tuning
- Logistic Regression provides fast, interpretable results
- Decision Trees offer excellent feature importance insights
- KNN works well with proper scaling and parameter selection

## Model Performance

| Algorithm | Accuracy | Precision | Recall | F1-Score |
|-----------|----------|-----------|--------|----------|
| Logistic Regression | 82% | 81% | 82% | 81% |
| Decision Trees | 85% | 84% | 85% | 84% |
| Random Forest | **89%** | **88%** | **89%** | **88%** |
| SVM | 86% | 85% | 86% | 85% |
| KNN | 84% | 83% | 84% | 83% |

*Note: Actual performance metrics may vary based on data split and hyperparameter tuning*

## Contributing

Contributions are welcome! If you'd like to improve this project, please:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature/improvement`)
6. Create a Pull Request

## License

This project is open source and available under the MIT License. See the LICENSE file for more details.

