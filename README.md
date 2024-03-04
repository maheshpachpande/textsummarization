# textsummarization project

# git clone
- git clone https://github.com/maheshpachpande/textsummarization.git

# create template.py
- python template.py

# create the vitual enviroment
- conda create -p textsummarization python==3.8 -y
- conda activate C:\Users\pachp\Desktop\project_git\textsummarization\textsummarization

# install requirements after setup.py file created
- pip install -r requirements.txt

# justifying how to work ensure_annotations, ConfigBox in trial.ipynb

# textsummurization.ipynb

# Workflows
- Update config.yaml
- Update params.yaml
- Update entity
- Update the configuration manager in src config
- update the conponents
- update the pipeline
- update the main.py
- update the app.py

#### Data-Ingestion (config -> config.yaml -> research -> 01_data_ingestion.ipynb -> entity -> configuration manager -> conponents -> pipeline -> main)

#### Data-Validation (config -> config.yaml -> research -> 02_data_validation.ipynb -> entity -> configuration manager -> conponents -> pipeline -> main)

#### Data-Transformation (config -> config.yaml -> research -> 03_data_transformation.ipynb -> entity -> configuration manager -> conponents -> pipeline -> main)

#### Model-Trainer (params.yaml -> config -> config.yaml -> research -> 04_model_trainer.ipynb -> entity -> configuration manager -> conponents -> pipeline -> main)

#### Model-Evaluation (config -> config.yaml -> research -> 05_model_evaluaion.ipynb -> entity -> configuration manager -> conponents -> pipeline -> main)

### Pipeline for prediction prediction.py

### appy.py


