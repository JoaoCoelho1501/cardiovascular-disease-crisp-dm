# Cardiovascular Disease Risk Classification — CRISP-DM and Amazon SageMaker

An end-to-end academic machine-learning project structured around the six phases of CRISP-DM, including model evaluation and deployment workflows using Amazon SageMaker.

**Academic context:** MSc in Business Intelligence & Analytics, ISCAP (2025/26)  
**Course:** Business Analytics — Tools and Applications  
**Authors:** Giulia Jacobina, João Coelho, and Larissa Tostes

## Project objective

The project investigates whether routinely collected health-related variables can support a binary classification task for cardiovascular disease risk.

The dataset includes variables such as age, blood pressure, cholesterol, and lifestyle indicators. The objective is to demonstrate an analytics workflow, not to provide a clinical diagnostic tool.

## CRISP-DM workflow

1. **Business understanding:** define the problem, objectives, research questions, and SWOT analysis.
2. **Data understanding:** inspect the data dictionary, missing values, duplicates, and potential outliers.
3. **Data preparation:** apply documented cleaning rules, feature engineering, and encoding.
4. **Modelling:** train and compare four classification models using a train/test split and appropriate preprocessing.
5. **Evaluation:** assess confusion matrices, ROC curves, AUC, accuracy, and feature importance.
6. **Deployment:** package the selected XGBoost model for Amazon SageMaker real-time inference and batch processing.

## Reported results

The project reports approximately **0.79 ROC-AUC** and **73% accuracy** for the selected model. Recall was considered an important selection criterion because false negatives can be consequential in a screening-oriented scenario.

These results are dataset- and split-specific and should not be interpreted as evidence of clinical validity.

## Technology stack

- Python, pandas, and scikit-learn
- XGBoost
- Amazon SageMaker and boto3
- Seaborn for exploratory visualisation

## Reproducing the project

The complete workflow and implementation details are documented in the project notebooks and report. Reproduction of the deployment stage requires an AWS account, appropriate IAM permissions, and configuration of the SageMaker environment.

Do not commit AWS access keys, secret keys, tokens, or other credentials to the repository. Use an approved local credentials profile or environment-based configuration.

## Scope and limitations

- This is an academic classification and deployment exercise, not a validated medical device.
- Dataset performance does not establish clinical usefulness, fairness, or generalisation to other populations.
- Any real-world health application would require clinical validation, governance, privacy safeguards, and oversight by qualified professionals.
- Cloud deployment may incur AWS charges; remove resources after testing.
