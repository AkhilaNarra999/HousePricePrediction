
# Real Estate Price Prediction and Analysis

This project focuses on analyzing real estate data from multiple cities to predict property prices using machine learning models. It also explores city-specific price trends, property characteristics, and relationships between various features.

---

## Table of Contents

1. [Overview](#overview)
2. [Dataset](#dataset)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Data Processing](#data-processing)
6. [Modeling](#modeling)
7. [City-Specific Analysis](#city-specific-analysis)


---

## Overview

This project combines property data from various cities, performs exploratory data analysis, and builds machine learning models to predict property prices. It includes city-specific analysis to identify localized trends and performance.

---

## Dataset

The dataset includes property details such as:

- **City**: Location of the property.
- **Price**: Property price (target variable).
- **Area**: Area of the property.
- **No. of Bedrooms**: Number of bedrooms in the property.
- **Resale**: Whether the property is a resale or not.
- **Amenities**: Features like gym, swimming pool, clubhouse, security, etc.

Additional features related to amenities and property details are used for analysis and modeling.

---

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/real-estate-price-prediction
   cd real-estate-price-prediction
   ```

2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Place the property dataset files (CSV) in the `dataset/` directory.

---

## Usage

Run the script in jupyter notebook to perform data preprocessing, visualization, and modeling:
```bash
code_version_2.ipynb
```

---

## Data Processing

1. Combine multiple city-specific datasets into a single dataset with a new column indicating the city.
2. Check for missing values and handle them using `SimpleImputer`.
3. Feature engineering:
   - Create `PricePerBedroom` for normalization.
   - Calculate the `TotalAmenities` by summing binary amenity columns.
4. Split the data into training and testing sets (80%/20%).

---


---

## Modeling

The following models are implemented:
1. **Linear Regression**
2. **Ridge Regression**
3. **Lasso Regression**
4. **Decision Tree**
5. **Random Forest**
6. **Gradient Boosting**

Evaluation metrics:
- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**

---

## City-Specific Analysis

The project performs separate modeling for each city to identify localized trends:
1. Train and test models on city-specific datasets.
2. Compare model performance metrics (MAE, MSE, RMSE) for each city.

---


