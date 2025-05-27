# Pyrolysis Data Analysis

Pyrolysis is a thermochemical conversion process used for the production of biofuels such as biochar, bio-oil, and syngas. The quality and yield of products obtained during biomass pyrolysis are dependent on several factors, such as biomass composition (proximate and ultimate analysis) and reaction conditions (temperature, heating rate, time). Therefore, it is imperative to understand the relationship between biomass composition, reaction conditions, and product yield during biomass pyrolysis.

## Project Overview

This project employs a data-driven machine learning (ML) and interpretability approach to study the complex relationships between biomass composition, reaction conditions, and product yield in the context of pyrolysis. Additionally, we aim to make the findings interpretable, as many ML models are often regarded as black boxes.

## Key Findings

- Several machine learning models were compared to assess their performance in this context.
- Out-of-the-box models for Random Forest (RF), XGBoost, Artificial Neural Networks (ANN), and Gradient Boosting Regressor (GBR) performed exceptionally well and did not benefit significantly from hyperparameter optimization.
- In contrast, the performance of Stochastic Gradient Descent (SGD) and AdaBoost models improved substantially after hyperparameter optimization.
- The Gradient Boosting Regressor (GBR) model outperformed all other models due to its ability to handle various types of data and capture non-linear connections and interactions between variables.
- A notable conclusion from the permutation feature importance analysis is that the oxygen (O) content had the most impact on various parameters, including H/C ratio, O/C ratio, gas yield, oil yield, and biochar yield. This was closely followed by the pyrolysis temperature (PT).

## Getting Started
1. Clone this repository to your local machine.
2. Install the necessary dependencies using `pip install -r requirements.txt`.
3. Explore the Jupyter notebooks in the main.ipynb for detailed analysis and findings.

## Note
- The data.xlsx in the datasets folder contains the raw data from the online source mentioned in the acknowledgment section.
- The dataset.xlsx in the datasets folder contains the transformed and preprocessed data used in this thesis.
- Finally, the clean_data.xlsx contains the cleaned data used in this research

## Acknowledgments
- Dr.Jude Okolie (University of Oklahoma, Gallogly College of Engineering) and M.sc Stell(Hochschule Bremerhaven) for their support and supervision
- The data used in this research is a combination of process simulation and literature as shown in the diagram below:
 ![IMG-20231121-WA0001](https://github.com/DouglasDivine/Thesis/assets/48439707/6abefdf6-04ef-429c-a087-dae784e9cc91)

- link to the trained model and deployed app on hugging face space: https://huggingface.co/spaces/DTonye/Waste-Biomass-Pyrolysis-Predictor

