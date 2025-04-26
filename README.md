# Walmart Time Series Sales Prediction

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python Version](https://img.shields.io/badge/python-3.10-blue)](https://www.python.org/downloads/)
[![PySpark](https://img.shields.io/badge/PySpark-3.3.0-orange)](https://spark.apache.org/docs/latest/api/python/index.html)

## 📊 Project Overview

A big data analytics project utilizing PySpark and machine learning to predict weekly sales across 45 Walmart stores. This implementation leverages time series forecasting techniques with Random Forest Regression to analyze historical sales patterns along with environmental and economic factors.

![Walmart Analytics](https://img.shields.io/badge/Walmart-Analytics-blue)

## 🔍 Features

- **Big Data Processing**: Efficiently handles large retail datasets with PySpark
- **ML Implementation**: Applies Random Forest Regression for sales forecasting
- **Data Quality Management**: Comprehensive validation and cleaning procedures
- **Statistical Analysis**: Examines correlations between sales and various factors

## 📈 Dataset

The analysis uses the Walmart dataset containing:

- `Store`: Store number (1-45)
- `Date`: Week of sales
- `Weekly_Sales`: Sales for the given store
- `Holiday_Flag`: Boolean indicating holiday week
- `Temperature`: Average temperature in the region
- `Fuel_Price`: Cost of fuel in the region
- `CPI`: Consumer Price Index
- `Unemployment`: Unemployment rate

## 🛠️ Tech Stack

- **PySpark**: For distributed big data processing
- **ML Libraries**: PySpark ML for model building
- **Jupyter Notebooks**: For interactive analysis and visualization
- **Python**: Core programming language

## 📋 Requirements

```
pyspark>=3.0.0
pandas>=1.3.0
numpy>=1.20.0
matplotlib>=3.4.0
seaborn>=0.11.0
```

## 🚀 Getting Started

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/walmart-sales-prediction.git
cd walmart-sales-prediction

# Create virtual environment (optional)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### Usage

```bash
# Run the data preprocessing
python src/preprocess.py

# Train the model
python src/train_model.py

# Generate predictions
python src/predict.py
```

## 📁 Project Structure

```
walmart-sales-prediction/
├── data/                     # Data directory
│   └── walmart-sales-dataset-of-45stores.csv
├── notebooks/                # Jupyter notebooks
│   └── easy.ipynb            # Main analysis notebook
├── src/                      # Source code
├── models/                   # Saved models
├── results/                  # Analysis results
├── requirements.txt          # Dependencies
└── README.md                 # This file
```

## 📝 Methodology

1. **Data Preparation**
   - Loading CSV data through PySpark
   - Schema validation and type conversion
   - Missing value detection

2. **Exploratory Analysis**
   - Distribution analysis of weekly sales
   - Correlation studies with environmental factors
   - Holiday impact assessment

3. **Feature Engineering**
   - Feature selection using Random Forest importance
   - Vector assembly for ML model input

4. **Model Training**
   - Random Forest Regressor implementation
   - Hyperparameter tuning
   - Cross-validation for model evaluation

## 📊 Results

The implementation successfully predicts weekly sales with insights into:
- Seasonal patterns affecting retail performance
- Impact of economic indicators on consumer behavior
- Store-specific factors influencing sales variations

## 🔄 Future Work

- Implement time series specific algorithms (ARIMA, Prophet)
- Develop interactive visualization dashboard
- Incorporate additional external data sources
- Deploy model as a microservice

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Walmart for providing the dataset
- Apache Spark community for the powerful data processing framework
