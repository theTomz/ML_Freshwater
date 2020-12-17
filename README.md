# ML_Freshwater
Repository for ML project 2: Improving Freshwater Quality Measurements through Machine Learning

- File Descriptions:
  - sdo1: Plynlimon study data set
  - UHF: 7-hour edited Plynlimon study values from UHF station (used for model fitting)
  - logistic_regression_and_ridge_regression: First model implementations (3 features) to compare regression techniques efficiency.
  - Gradient_Descent: Regression model using Least Squares Gradient Descent.
  - Normalized gradient descent: Regression model with normalized outputs to compare efficiency between different ions.
  - Create_Excel: Code to generate features for the neural network.
  - Neural_Network: Neural Network implementation.

- How To Run
  - Gradient_Descent and Normalized_Gradient_Descent: Self-contained, all functions needed are in the code. Running the notebook will provide outputs and pyplot comparisons of prediction and actual samples.
    - To test with different ions, replace variable "ion" with desired component (must be a column header of UHF data set). Outputs are at the bottom of the code (see pyplot for predictions).
    - To switch between sampling intervals, replace value "Time_between_samples" with desired interval in days.
  - Neural Network: Create input excels first by running the "Create_Excel" file.
    - To switch between ions, replace variable "ion" with desired component (must be a column header of UHF data set). Outputs are at the bottom of the code (see pyplot for predictions).
    - To switch between sampling intervals, replace value "Time_between_samples" with desired interval in days.
    Run neural network by replacing variable "features" with: 'new_features' + str(Time_between_sample) + '.xlsx'. 
    Neural Network outputs pyplot prediction compared to test samples.
