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


#### AWS-CICD-Deployment-with-Github-Actions
1. Login to AWS console.
2. Create IAM user for deployment
#### with specific access

1. EC2 access : It is virtual machine

2. ECR: Elastic Container registry to save your docker image in aws


#### Description: About the deployment

1. Build docker image of the source code

2. Push your docker image to ECR

3. Launch Your EC2 

4. Pull Your image from ECR in EC2

5. Lauch your docker image in EC2

#### Policy:

1. AmazonEC2ContainerRegistryFullAccess

2. AmazonEC2FullAccess
3. Create ECR repo to store/save docker image
- Save the URI: 566373416292.dkr.ecr.us-east-1.amazonaws.com/text-s
4. Create EC2 machine (Ubuntu)
5. Open EC2 and Install docker in EC2 Machine:
#### optinal

- sudo apt-get update -y

- sudo apt-get upgrade

#### required

- curl -fsSL https://get.docker.com -o get-docker.sh

- sudo sh get-docker.sh

- sudo usermod -aG docker ubuntu

- newgrp docker
6. Configure EC2 as self-hosted runner:
setting>actions>runner>new self hosted runner> choose os> then run command one by one
7. Setup github secrets:
- AWS_ACCESS_KEY_ID=

- AWS_SECRET_ACCESS_KEY=

- AWS_REGION = us-east-1

- AWS_ECR_LOGIN_URI = demo>>  566373416292.dkr.ecr.ap-south-1.amazonaws.com

- ECR_REPOSITORY_NAME = simple-app


