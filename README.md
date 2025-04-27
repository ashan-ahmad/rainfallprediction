# Rainfall Prediction Classifier

This project is a machine learning pipeline designed to predict whether it will rain today based on historical weather data. The dataset used for this project is sourced from the Australian Government's Bureau of Meteorology and Kaggle.

## Table of Contents
- [About the Dataset](#about-the-dataset)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Modeling Approach](#modeling-approach)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## About the Dataset

The dataset contains daily weather observations from 2008 to 2017 across various locations in Australia. It includes features such as temperature, rainfall, humidity, wind speed, and more. The target variable is whether it rained today (`RainToday`).

### Dataset Source:
- [Kaggle Dataset](https://www.kaggle.com/datasets/jsphyg/weather-dataset-rattle-package)
- [Bureau of Meteorology](http://www.bom.gov.au/climate/dwo/)

## Features

The dataset includes the following key features:
- **Date**: Date of observation.
- **Location**: Observation location.
- **MinTemp**: Minimum temperature (°C).
- **MaxTemp**: Maximum temperature (°C).
- **Rainfall**: Amount of rainfall (mm).
- **WindGustDir**: Direction of the strongest wind gust.
- **Humidity9am**: Humidity at 9 AM (%).
- **RainToday**: Whether it rained today (Yes/No).

For a full list of features, refer to the notebook.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/rainfall-prediction-classifier.git
   cd rainfall-prediction-classifier
   ```

2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Open the Jupyter Notebook:
   ```bash
   jupyter notebook Rainfall_Prediction_Classifier.ipynb
   ```

2. Follow the steps in the notebook to preprocess the data, train the model, and evaluate its performance.

## Modeling Approach

The project uses a machine learning pipeline with the following steps:
1. **Data Preprocessing**:
   - Handle missing values.
   - Feature engineering (e.g., creating a `Season` feature from the `Date` column).
   - One-hot encoding for categorical variables.
   - Standard scaling for numerical variables.

2. **Model Training**:
   - Random Forest Classifier and Logistic Regression models are trained using a pipeline.
   - Hyperparameter tuning is performed using GridSearchCV with cross-validation.

3. **Evaluation**:
   - Classification metrics such as accuracy, precision, recall, and F1-score.
   - Confusion matrix visualization.
   - Feature importance analysis.

## Results

- The Random Forest Classifier achieved a cross-validation accuracy of approximately **X%**.
- The Logistic Regression model achieved a cross-validation accuracy of approximately **Y%**.
- The dataset is imbalanced, with the "No" class significantly outweighing the "Yes" class.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
