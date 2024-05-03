# Student_Performance_Indicator_AWS_CI-CD

#  Components

Data Ingestion is apart of components module which means reading dataset from databases/file locations

Ingested data is transformed inside data_transformation.py

Model Training will happen in model_trainer.py

Logger has all the log files

Exception handling is taking care by exception.py, exc_info() tells the file name and line number where the exception is occuring

# DataIngestionConfig is input component to Data Ingestion

# End to End MAchine Learning Project

Docker Build checked
Github Workflow
Iam User In AWS
Docker Setup In EC2 commands to be Executed
#optinal

sudo apt-get update -y

sudo apt-get upgrade

#required

curl -fsSL https://get.docker.com -o get-docker.sh

sudo sh get-docker.sh

sudo usermod -aG docker ubuntu

newgrp docker

# Configure EC2 as self-hosted runner:

Setup github secrets:

AWS_ACCESS_KEY_ID=

AWS_SECRET_ACCESS_KEY=

AWS_REGION = us-east-1

AWS_ECR_LOGIN_URI = demo>> 566373416292.dkr.ecr.ap-south-1.amazonaws.com

ECR_REPOSITORY_NAME = simple-app

