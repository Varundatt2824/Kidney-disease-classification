# Kidney-Disease-Classification-MLflow-DVC


## Workflows

1. Update config.yaml
2. Update params.yaml
3. Update the entity
4. Update the configuration manager in src config
5. Update the components
6. Update the pipeline 
7. Update the main.py
8. Update the dvc.yaml
10. app.py

# How to run?
### STEPS:

Clone the repository

```bash
https://github.com/Varundatt2824/Kidney-disease-classification
```
### STEP 01- Create a conda environment after opening the repository

```bash
conda create -n kidney python=3.8 -y
```

```bash
conda activate kidney
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






## MLflow

- [Documentation](https://mlflow.org/docs/latest/index.html)

- [MLflow tutorial](https://youtu.be/qdcHHrsXA48?si=bD5vDS60akNphkem)

##### cmd
- mlflow ui

### dagshub
[dagshub](https://dagshub.com/)

set MLFLOW_TRACKING_URI=https://dagshub.com/Varundatt2824/Kidney-disease-classification.mlflow


set MLFLOW_TRACKING_USERNAME=Varundatt2824


set MLFLOW_TRACKING_PASSWORD=3a44f275bb0efc0ab1407b3a010755c84996f34a


python script.py

Run this to export as env variables:

```bash
#use set instead of export in case of windows
export MLFLOW_TRACKING_URI=https://dagshub.com/Varundatt2824/Kidney-disease-classification.mlflow

export MLFLOW_TRACKING_USERNAME=Varundatt2824

export MLFLOW_TRACKING_PASSWORD=3a44f275bb0efc0ab1407b3a010755c84996f34a

```


### DVC cmd

1. dvc init
2. dvc repro
3. dvc dag


## About MLflow & DVC

MLflow

 - Its Production Grade
 - Trace all of your expriements
 - Logging & taging your model


DVC 

 - Its very lite weight for POC only
 - lite weight expriements tracker
 - It can perform Orchestration (Creating Pipelines)


## AZURE-CICD-Deployment-with-Github-Actions
# Save pass:
s3cEZKH5yytiVnJ3h+eI3qhhzf9q1vNwEi6+q+WGdd+ACRCZ7JD6

# Run from terminal:
<acr-name>: azure cloud registry
docker build -t <acr-name>.azurecr.io/<image-name> .
docker tag image-name <acr-name>.azurecr.io/<image-name>
docker login <acr-name>.azurecr.io

docker push kidneyapp.azurecr.io/<image-name>

# Deployment Steps:
Build the Docker image of the Source Code
Push the Docker image to Container Registry
Launch the Web App Server in Azure
Pull the Docker image from the container registry to Web App server and run