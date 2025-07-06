# House Price Prediction: Data Preprocessing and Feature Engineering

This project involves cleaning, transforming, and engineering features from a real estate dataset to predict house prices using advanced regression techniques. 

##  Project Objectives

- Handle missing values and data inconsistencies.
- Convert categorical variables to numerical format using encoding techniques.

##  Dataset Description

The dataset contains information about residential homes in Ames, Iowa. Each row represents a property sale and includes over 80 explanatory variables describing aspects of residential homes.

**Target Variable**:
- `SalePrice`: The sale price of the house (log-transformed for modeling)

**Key Feature Groups**:
- **Categorical Variables**: Zoning, Neighborhood, House Style, etc.
- **Ordinal Variables**: Quality ratings (e.g., `ExterQual`, `KitchenQual`)
- **Numerical Variables**: Lot Area, Basement Size, Total Rooms, etc.
- **Engineered Features**: `TotalBathrooms`, `TotalPorchSF`, `HouseAge`, etc.

## Data Preprocessing

- Missing value treatment using median, mode, and custom logic by `Neighborhood`.
- Mapping of ordinal categorical features to integers.
- One-hot encoding of nominal categorical variables.
- Log transformation of highly skewed numerical features.
- Feature scaling using `StandardScaler`.

##  Feature Engineering

New features created:
- `TotalBathrooms`
- `TotalPorchSF`
- `HouseAge`
- `RemodelAge`
- `GarageAge`
- Binary flags for presence of features: `HasGarage`, `HasFireplace`, `HasPool`, etc.
