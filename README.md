
# Coronary Artery Disease Prediction from CT Scans


## Project Overview
Automated CAD risk prediction using:
1. DICOM CT preprocessing
2. Cardiac ROI extraction
3. Calcium segmentation
4. 3D CNN risk modeling

## Installation
```bash
git clone https://github.com/yourusername/cad-prediction.git
cd cad-prediction
pip install -r requirements.txt
Usage
Data Preparation

python
from data_processing.dicom_to_hu import load_dicom_hu
hu, dicom = load_dicom_hu("ct.dcm")
Training

python
from model.train_3dcnn import train_model
model = train_model(ct_volumes, labels)
Prediction

python
from model.predict import predict_risk
risk = predict_risk(model, ct_volume, clinical_data)
File Structure
/data_processing: DICOM conversion and ROI extraction

/model: 3D CNN training/prediction

/utils: Visualization tools

Requirements
Python 3.8+

PyTorch 1.10+

MONAI 0.9+

pydicom 2.3+

References
RSNA Pulmonary Embolism Dataset

MONAI U-Net Architecture

Agatston Scoring Protocol

text

---

### **requirements.txt**
pydicom>=2.3.0
numpy>=1.21.0
torch>=1.10.0
monai>=0.9.0
scikit-image>=0.19.0
matplotlib>=3.5.0
seaborn>=0.11.2

text

---

### **Key Features**
1. **End-to-End Pipeline**: DICOM → Risk Prediction
2. **Modular Design**: Easy to swap components
3. **Clinical Readiness**: Includes Agatston scoring
4. **Explainability**: SHAP values and Grad-CAM

To run the complete workflow:
```bash
python -m data_processing.dicom_to_hu input.dcm
python -m model.train_3dcnn
python -m model.predict sample_ct.npy  give this readme file for direct copy paste to github
