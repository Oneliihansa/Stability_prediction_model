
# Project Title

The primary goal of this project is to develop a machine learning model that can accurately
predict system stability (stab) of an electrical grid based on a variety of quantitative factors, such
as reaction times, power variables, and price elasticity coefficients. With this goal in mind, I
framed the approach as a regression problem due to the continuous nature of the target variable,
stab.


## Target Variable and Features


• Target Variable: The target variable is stab, a continuous variable representing system
stability. Positive values of "stab" indicate an unstable state, while negative values signify
a stable state.
• Features: The dataset contains 13 numerical features (tau1-tau4, p1-p4, g1-g4),
representing factors such as reaction times, power variables, and price elasticity.

1. Reaction Times (tau1 to tau4): These variables measure different reaction times within
the system, potentially reflecting how the system responds to changes. Longer or shorter
reaction times can impact stability.

2. Power Variables (p1 to p4): These represent various power-related metrics, such as
power input, output, or internal energy levels. Power fluctuations or sustained power
levels can affect system balance, contributing to stability or instability depending on how
energy is managed.

3. Price Elasticity Coefficients (g1 to g4): These variables represent price elasticity within
the system. Elasticity indicates how sensitive a system is to changes in price or demand.
Here, these coefficients could reflect how responsive the system is to external changes,
potentially impacting stability.
## Tuning Method:

Hyperparameters were optimized using Grid Search, with tuning for parameters like max_depth, min_samples_split, n_estimators, C across models. Each model was reevaluated post-tuning to assess improvement.

## Model Selection and Baseline Establishment
Given the regression task, we selected five different models to understand which best captures the patterns in stab:

• Linear Regression: A simple, interpretable model serving as a baseline.

• Decision Tree: A non-linear model that partitions data into segments, suitable for capturing complex patterns but prone to overfitting.

• Random Forest: An ensemble of decision trees offering improved accuracy and reduced overfitting compared to a single tree.

• Support Vector Regression (SVR): A margin-based model that seeks to minimize errors within a defined boundary.

• Gradient Boosting: An ensemble model that builds sequential models to correct errors, effective in capturing non-linear patterns.
