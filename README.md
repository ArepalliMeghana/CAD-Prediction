# Coronary Artery Disease Prediction

This project predicts the likelihood of Coronary Artery Disease (CAD) using machine learning models trained on patient data. The system utilizes cleaned datasets and a pre-trained model to assess risks and generate insights.

## Features
- **Dataset Handling**: Cleaned CSV and Excel files for patient records.
- **Model**: Pre-trained Decision Tree model (`DT-cyber.pkl`).
- **Implementation**: Python-based analysis using a Jupyter Notebook.

## Project Structure
```
CAD-Prediction-main/
│
├── Cardiac_cleaned_data.csv                  # Cleaned dataset in CSV format
├── Cardiac_disease.ipynb                     # Main implementation notebook
├── DT-cyber.pkl                              # Pre-trained machine learning model
└── Patients Information Of Cardiac Dataset.xlsx  # Supplementary patient information
```

## How to Run the Project
1. Clone this repository:
   ```bash
   git clone <repository-link>
   cd CAD-Prediction-main
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open the Jupyter notebook:
   ```bash
   jupyter notebook Cardiac_disease.ipynb
   ```
4. Follow the steps in the notebook to execute the code and analyze results.

## Dependencies
- Python 3.x
- Jupyter Notebook
- Required libraries (listed in `requirements.txt`)

## Future Enhancements
- Extend the system with a symptom checker.
- Provide comprehensive health reports with lifestyle and dietary recommendations.
- Implement decision support for medication or surgery based on disease severity.


