# Life Expectancy Prediction System

A machine learning system that predicts life expectancy based on various health, economic, and demographic factors using Artificial Neural Networks.

## What It Does

- **Life Expectancy Prediction**: Estimates average life expectancy based on multiple factors
- **Neural Network**: Uses ANN for accurate predictive modeling
- **Data Analysis**: Comprehensive analysis of factors affecting longevity
- **Health Analytics**: Insights into health determinants

## Quick Start

```bash
# Install dependencies
pip install pandas numpy scikit-learn tensorflow matplotlib seaborn

# Run the analysis
jupyter notebook LIFE_EXPECTANCY_Asmaa.mz.ipynb
```

## Project Structure

```
ANN-Predict-_life-Expectancy/
    LIFE_EXPECTANCY_Asmaa.mz.ipynb    # Main analysis and model training
    ANN_Task.csv                     # Dataset with health indicators
    README.md                        # This file
```

## Dataset Information

### Features
- **Health Indicators**: Mortality rates, health expenditures
- **Economic Factors**: GDP, income levels, education
- **Demographics**: Population statistics, age distribution
- **Lifestyle Factors**: Alcohol consumption, BMI, etc.

### Target Variable
- **Life Expectancy**: Average life expectancy in years

## Model Architecture

### Neural Network Design
- **Input Layer**: Multiple health and economic features
- **Hidden Layers**: Optimized ANN architecture
- **Output Layer**: Life expectancy prediction
- **Activation**: ReLU for hidden layers, linear for output

### Training Process
1. **Data Preprocessing**: Handle missing values, normalize features
2. **Feature Engineering**: Create meaningful predictors
3. **Model Training**: ANN with backpropagation
4. **Validation**: Cross-validation for robustness
5. **Evaluation**: Performance metrics and analysis

## Technical Specifications

### Dependencies
```
pandas>=1.3.0
numpy>=1.20.0
scikit-learn>=1.0.0
tensorflow>=2.0.0
matplotlib>=3.0.0
seaborn>=0.11.0
jupyter>=1.0.0
```

### Model Details
- **Algorithm**: Artificial Neural Network (ANN)
- **Framework**: TensorFlow/Keras
- **Input Features**: Multiple health/economic indicators
- **Output**: Continuous life expectancy value
- **Loss Function**: Mean Squared Error
- **Optimizer**: Adam

## Data Analysis

### Exploratory Data Analysis
- **Feature Distribution**: Analysis of variable distributions
- **Correlation Analysis**: Relationships between factors
- **Missing Values**: Data quality assessment
- **Outlier Detection**: Identify anomalies

### Key Insights
- **Health Impact**: How health indicators affect longevity
- **Economic Factors**: Economic development and life expectancy
- **Regional Differences**: Geographic variations
- **Temporal Trends**: Changes over time

## Model Performance

### Evaluation Metrics
- **Mean Absolute Error**: Average prediction error
- **Mean Squared Error**: Overall model accuracy
- **R-squared**: Explained variance
- **Cross-validation**: Model robustness

### Feature Importance
- **Health Expenditure**: Impact of healthcare spending
- **Economic Development**: GDP and income effects
- **Education**: Educational attainment influence
- **Lifestyle**: Behavioral factors

## Applications

### Public Health
- **Policy Planning**: Inform health policy decisions
- **Resource Allocation**: Optimize healthcare spending
- **Targeted Interventions**: Focus on high-risk areas
- **Health Monitoring**: Track population health

### Research
- **Epidemiological Studies**: Population health research
- **Comparative Analysis**: Cross-country comparisons
- **Trend Analysis**: Monitor changes over time
- **Risk Assessment**: Identify health risks

## Usage Guide

### Data Preparation
```python
import pandas as pd

# Load dataset
data = pd.read_csv('ANN_Task.csv')

# Preprocess
# Handle missing values
# Normalize features
# Split data
```

### Model Training
```python
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Dense

# Build ANN model
model = Sequential([
    Dense(64, activation='relu', input_shape=(n_features,)),
    Dense(32, activation='relu'),
    Dense(16, activation='relu'),
    Dense(1, activation='linear')
])

# Compile and train
model.compile(optimizer='adam', loss='mse')
model.fit(X_train, y_train, validation_split=0.2)
```

### Prediction
```python
# Make predictions
predictions = model.predict(X_test)

# Evaluate performance
from sklearn.metrics import mean_absolute_error
mae = mean_absolute_error(y_test, predictions)
```

## Key Findings

### Major Factors
- **Healthcare Access**: Quality and availability of healthcare
- **Economic Development**: GDP per capita impact
- **Education**: Educational attainment levels
- **Lifestyle**: Diet, exercise, and habits

### Regional Variations
- **Developed Countries**: Higher life expectancy
- **Developing Nations**: Improving trends
- **Healthcare Systems**: System effectiveness
- **Social Factors**: Community and social support

## Future Enhancements

- **Deep Learning**: Advanced neural architectures
- **More Features**: Additional health indicators
- **Time Series**: Temporal prediction models
- **Geographic Analysis**: Spatial modeling
- **Real-time Data**: Live data integration

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

This project is licensed under the MIT License.

## Acknowledgments

- **WHO Data**: World Health Organization health statistics
- **World Bank**: Economic development indicators
- **UN Data**: United Nations demographic data

---

**Predicting healthier futures with AI!**
