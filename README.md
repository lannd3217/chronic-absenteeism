# Chronic Absenteeism Data Exploration and Prediction
## Project Description
This project analyzes and predicts chronic absebteeism among students in schools within the Oakland District. By leveraging historical attendance, demographics, and academic data, we build machine learning models to predict absenteeism risks and provide insights for early intervention.
The project consists of two main components:
1. Data Exploration - Cleaning, transforming, and analyzing student data.
2. Prediction Models - Implementating machine learning models to predict absenteeism for the next academic year.

## Installation Instructions
To run this project locally, install the required dependences using
pip install pandas numpy matplotlib seaborn scikit-learn jupyter

If using Google Colab, mount Google Drive
from google.colab import drive
drive.mount('/content/drive')

## Usage Instructions
### 1. Data Exploration
- Load the dataset from `data/` using `pandas.read_csv()`.
- Clean and preprocess data:
  - Handle missing values in key columns (e.g., `Susp`, `Gen`, `AttRate`).
  - Standardize categorical values.
  - Compute additional features (e.g., student age, absenteeism indicator).
- Generate visualizations to understand trends in attendance and absenteeism.

### 2. Predicting Chronic Absenteeism
- Train machine learning models using historical student data.
- Two models are used:
  - Model 1: Predicts absenteeism for students below grade 6.
  - Model 2: Predicts absenteeism for students in grade 6 and above.
- Feature Engineering:
  - Past attendance records.
  - Demographic attributes.
  - GPA trends (for older students).
- Evaluate models with:
  - Accuracy, Precisison, Recall, F1-score
  - Confusion Matrix
  - Feature Importance Analysis
  - ROC Curve & AUC Score
- Predict at-risk students for the upcoming school year.

## Contributors
Lan Dinh


## File Structure
📂 chronic-absenteeism

│── 📁 data/              # Contains datasets for multiple schools and years

│── 📁 notebooks/         # Jupyter Notebooks for data exploration and model training

│── 📁 reports/           # Analysis reports in PDF and HTML format

│── 📄 README.md          # Project documentation (this file)


