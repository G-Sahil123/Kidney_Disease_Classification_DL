# Kidney-Disease-Classification-MLflow-DVC

## **Table of Contents**
- [Project Overview](#project-overview)  
- [Features](#features)  
- [Project Structure](#project-structure)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Data](#data)  
- [Pipeline Stages](#pipeline-stages)  
- [MLflow Integration](#mlflow-integration)  
- [CI/CD Deployment](#cicd-deployment)  
- [Contributing](#contributing)  
- [License](#license)  

---

## **Project Overview**
Kidney disease detection is critical for early diagnosis and treatment. This project leverages **deep learning** to automate classification of kidney CT scan images into:  

1. **Normal**  
2. **Cyst**  
3. **Tumor**  
4. **Stone**  

We use **transfer learning** with pre-trained CNN model VGG16 to improve accuracy.

---

## **Features**
- **CNN-based classification** using transfer learning  
- **Modular coding structure** for maintainable pipeline  
- **DVC** for dataset and model versioning  
- **MLflow** for experiment tracking (metrics, parameters, artifacts)  
- **CI/CD pipeline** for automatic deployment of trained models  
- **Configurable hyperparameters** using `config.yaml` and `params.yaml`  

---

## Workflows

1. Update config.yaml
2. Update params.yaml
3. Update the entity
4. Update the configuration manager in src config
5. Update the components
6. Update the pipeline 
7. Update the main.py
8. Update the dvc.yaml
9. app.py

# How to run?
### STEPS:

Clone the repository

```bash
https://github.com/G-Sahil123/Kidney_Disease_Classification_DL.git
cd Kidney_Disease_Classification
```
### STEP 01- Create a virtual environment after opening the repository

```bash
python -m venv myvenv
# Windows
myvenv\Scripts\activate
# Linux/macOS
source myvenv/bin/activate
```

### STEP 02- install the requirements
```bash
pip install -r requirements.txt
```

```bash
# Finally run the following command
python app.py
```

Now,
```bash
open up you local host and port
```

## Usage
### Run the full pipeline
```bash
dvc repro
```
This will execute all stages sequentially
1. Data ingestion
2. Base model preparation
3. Model Training
4. Evaluation

## MLflow

- [Documentation](https://mlflow.org/docs/latest/index.html)

- [MLflow tutorial](https://youtu.be/qdcHHrsXA48?si=bD5vDS60akNphkem)

```bash
  mlflow ui
``` 


