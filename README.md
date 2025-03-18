# Machine_Learning_2023_OVGU

## Description
**Machine Learning for Chemical Engineering**  
Welcome to the course on Machine Learning for Chemical Engineering! In this course, we explore the fascinating intersection of machine learning and chemical engineering, understanding how these two fields can synergistically solve complex problems and optimize processes in the chemical industry.

## How to Use the Notebook
1. **Open the Notebook:**  
   Launch the Jupyter Notebook:
   ```bash
   jupyter notebook <notebook_filename>.ipynb
   ```
2. **Follow the Structured Workflow:**  
   The notebook is organized into clearly defined sections with detailed markdown explanations and in-code comments. Each section includes data cleaning, feature engineering, model development, cross-validation, visualization, and model saving steps.

## Class Tasks

### Task 1/2: kNN Regression for BCF Prediction

#### Objective
Develop a k-Nearest Neighbors (kNN) regression model to predict the Bioconcentration Factor (BCF) using the provided chemical dataset. The goal is to determine the optimal number of neighbors (k) by evaluating the model's performance with cross-validation.

#### Detailed Explanation
- **Data Cleaning & Preprocessing:**  
  The dataset may contain missing or inconsistent values. We perform necessary cleaning and preprocessing, and define the variables:
  - **Inputs/Features:** All relevant chemical descriptors.
  - **Output:** Experimental values representing log(Bioconcentration Factor) in L/kg.
- **Cross-Validation:**  
  Multiple k values are tested using cross-validation. We visualize performance metrics such as R² (coefficient of determination) and MSE (Mean Squared Error) versus different k values.
- **Model Training:**  
  Once the optimal k is selected, the final model is trained on the entire dataset.

#### Dataset Information
The dataset for Task 1/2 contains the following column headings:
- **CAS**
- **SMILES**
- **Experimental value [log(L/kg)]**
- **NumAromaticRings**
- **NumHAcceptors**
- **NumHeteroatoms**
- **NumRotatableBonds**
- **NumValenceElectrons**
- **qed**
- **TPSA**
- **MolMR**
- **BalabanJ**
- **BertzCT**
- **fr_COO**
- **fr_COO2**
- **fr_halogen**
- **MolWt**
- **MolLogP**

### Task 3: Generalized Linear Regression for Internal Energy Prediction

#### Objective
Develop a Generalized Linear Regression model to predict the Internal Energy (U) of saturated vapor based on pressure data. The objective is to identify the best polynomial degree through cross-validation that results in the most accurate predictions.

#### Detailed Explanation
- **Data Cleaning & Preprocessing:**  
  The dataset is examined for missing values and inconsistencies. The variables are defined as:
  - **Input/Feature:** Pressure data.
  - **Output:** Internal Energy values for saturated vapor.
- **Cross-Validation:**  
  We perform cross-validation by testing various degrees of the polynomial regression model. Visualizations of R² and MSE against the degree of the polynomial help in determining the optimal degree.
- **Model Training:**  
  The final model is trained using the optimal polynomial degree on the entire dataset, ensuring robust predictions for Internal Energy.

#### Dataset Information
The dataset for Task 3 contains the following column headings(The dataset is in a pivot for better analysis):
- **Pressure**
- **Property**
- **Liq_Sat**
- **Vap_Sat**
- **75**
- **100**
- **125**
- **150**
- **175**
- **200**
- **220**
- **225**
- **240**
- **250**
- **260**
- **275**
- **280**
- **290**
- **300**
- **320**
- **325**
- **340**
- **350**
- **360**
- **375**
- **380**
- **400**
- **425**
- **450**
- **475**
- **500**
- **525**
- **550**
- **575**
- **600**
- **625**
- **650**

### Task 4: Deep Neural Network for Electric Power (PE) Prediction

#### Objective
Develop a Deep Neural Network (DNN) using PyTorch to predict Electric Power (PE) in a Combined Cycle Power Plant (CCPP). The model uses various plant parameters to forecast the electric output with high accuracy.

#### Detailed Explanation
- **Data Cleaning & Preprocessing:**  
  The dataset is cleaned, and variables are defined:
  - **Inputs/Features:** Ambient Temperature (AT), Exhaust Vacuum (V), Atmospheric Pressure (AP), Relative Humidity (RH).
  - **Output:** Electric Power (PE).
- **Model Development:**  
  A Feed Forward Neural Network is constructed using PyTorch. The network’s architecture is designed to capture non-linear relationships between inputs and output.
- **Cross-Validation with GridSearchCV:**  
  GridSearchCV is employed to optimize hyperparameters, ensuring the best model configuration.
- **Final Model Training & Saving:**  
  The final DNN model is trained on the entire dataset using the optimized hyperparameters. The final optimized model is then saved in a  `final_model.h5`.
- **Test Function:**  
  A function is written to get the saved model and test it on a new set of data. This way the model is reusable and can be deployed.

#### Dataset Information
The dataset for Task 4 contains the following column headings:
- **AT** (Ambient Temperature)
- **V** (Exhaust Vacuum)
- **AP** (Atmospheric Pressure)
- **RH** (Relative Humidity)
- **PE** (Electric Power)

## Results/Findings
- **Task 1/2:** Optimal k selection for kNN Regression on BCF prediction.
- **Task 3:** Best polynomial degree selection for accurate Internal Energy predictions.
- **Task 4:** Optimized DNN model for Electric Power forecasting.

## Future Work
- Explore additional algorithms like SVM and Random Forest.
- Improve feature engineering and dataset augmentation.
- Deploy models into production environments.

## License Information
This project is licensed under the MIT License.

## Author
Joseph Ishola

