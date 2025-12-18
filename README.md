# Identifying Key Predictors of Diabetes Progression
The purpose of this project is to use interpretable machine learning models to understand how different features influence progression using Diabetes dataset from scikit-learn. By knowing the most important variables, clinicians can identify what patient is at risk. 
Three complementary regression models are trained and compared:
- Linear regression
- Random Forest Regressor
- Gradient Boosting Regressor

## Objectives
Predict diabetes disease progression using clinical features
Compare performance across multiple regression models
Interpret model behavior using:
- Coefficients
- Feature importance
- Permutation importance
- Partial Dependence Plots (PDPs)
Demonstrate the trade-off between accuracy and interpretability

## Dataset 
- Source: sklearn.datasets.load_diabetes
- Features: 10 standardized clinical variables
  - Age, sex, BMI, blood pressure
  - Six blood serum measurements
- Target: A quantitative measure of disease progression one year after baseline

## Evaluation Metrics
- Root Mean Squared Error (RMSE)
- R² Score

## How to Replicate This Project

### 1. Clone the Repository

   ```bash
git clone https://github.com/angelx34/csc334_finalproject.git
cd <csc334_finalproject>
```
### 2. Create a Python Enviroment 

   ```bash
conda create -n csc334 diabetes-ml python=3.10
conda activate csc334 diabetes-ml
```
## 3. Install Required Dependencies

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```
## 4. Run the Notebook

```bash
jupyter notebook 
```
```bash
finalproj.ipynb
```
## Conclusion 
BMI and serum measure s5 are the two most important predictors of diabetes progression
Random Forest and Gradient Boosting confirm these patterns and reveal important effects that couldn't be identified with a linear regression model.
The permutation importance test supports that the most important factors are s5 and BMI 
Blood Pressure and s6 are the next most important values while age and sex contribute little
