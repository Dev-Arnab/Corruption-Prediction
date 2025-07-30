# Corruption Perception Prediction

This project predicts the "Perceptions of Corruption" score for countries using features from the World Happiness Report dataset. The workflow follows the machine learning lifecycle: data loading, exploratory analysis, feature selection, model training, evaluation, and visualization.

## Dataset

- **Source:** World Happiness Report (`WHR2018Chapter2OnlineData.csv`)
- **Target Variable:** Perceptions of corruption
- **Features Used:**  
  - Delivery Quality  
  - Freedom to make life choices  
  - Confidence in national government  
  - Life Ladder  
  - Standard deviation/Mean of ladder by country-year  
  - Democratic Quality  
  - Generosity  

## Project Steps

1. **Data Loading:**  
   Load the World Happiness Report dataset and inspect its structure.

2. **Data Cleaning:**  
   Handle missing values and aggregate data by country.

3. **Feature Selection:**  
   Select the most relevant features using statistical methods and domain knowledge.

4. **Data Preparation:**  
   Scale features and split the data into training and test sets.

5. **Modeling:**  
   - Linear Regression  
   - XGBoost Regressor (with manual hyperparameter tuning)

6. **Evaluation:**  
   Evaluate models using R², MAE, and MAPE metrics.

7. **Visualization:**  
   - Model performance comparison (bar plots for R², MAE, MAPE)
   - Residual plots
   - Actual vs. predicted scatter plots
   - Feature importance bar plot

## Results

- XGBoost outperformed Linear Regression, achieving an R² greater than 0.7.
- Feature importance analysis highlights which factors most influence corruption perception.

## Requirements

- Python 3.9+
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- xgboost
- tensorflow (for parallel processing setup)

Install dependencies with:

```sh
pip install pandas numpy matplotlib seaborn scikit-learn xgboost tensorflow
```

## Usage

Open `DefineAndSolveMLProblem.ipynb` in Jupyter Notebook or VS Code and run the cells sequentially to reproduce the analysis and results.

## File Structure

- [DefineAndSolveMLProblem.ipynb](DefineAndSolveMLProblem.ipynb): Main notebook containing all code, analysis, and results.

## License

This project is for educational purposes.