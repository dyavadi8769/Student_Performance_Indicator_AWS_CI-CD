# This is a Machine Learning End-End Project


# Components

Data Ingestion is apart of components module which means reading dataset from databases/file locations

Ingested data is transformed inside data_transformation.py

Model Training will happen in model_trainer.py

Model prediction is occuring in predict_pipeline.py

Logger has all the log files

Exception handling is taking care by exception.py, exc_info() tells the file name and line number where the exception is occuring

# Steps for AWS Deployment

1. Create a user in AWS IAM .
2. Create a repository in AWS Elastic Container Registry.
3. Create an instance in AWS EC2.
4. Setup Docker in AWS EC2 instance.
5. Create Runner in GitHub, execute the commands step by step to  for Download, Configure, Use the self-Hosted Runner.

# Commands for setting up Docker in EC2 :

```
sudo apt-get update -y
```
```
sudo apt-get upgrade
```
```
curl -fsSL https://get.docker.com -o get-docker.sh
```
```
sudo sh get-docker.sh
```
```
sudo usermod -aG docker ubuntu
```
```
newgrp docker

```



# Configure EC2 as self-hosted runner:

Setup github secrets:

AWS_ACCESS_KEY_ID=

AWS_SECRET_ACCESS_KEY=

AWS_REGION = us-east-1

AWS_ECR_LOGIN_URI = demo>> 566373416292.dkr.ecr.ap-south-1.amazonaws.com

ECR_REPOSITORY_NAME = simple-app
