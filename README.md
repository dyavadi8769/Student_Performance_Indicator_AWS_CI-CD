## Student Performance Indicator

# This is a Machine Learning End-End Project


# Project Overview

This project develops a predictive model to assess student performance using machine learning regression techniques. Aimed at educational institutions, the model predicts academic outcomes based on students' demographic and academic data. The repository includes a full suite of scripts for data preprocessing, model training, prediction, and evaluation. Additionally, the project is configured for AWS deployment with CI/CD integration, ensuring scalability and ease of updates. This approach enhances decision-making and strategic planning in education by providing actionable insights into student performance.

# Steps Involved

1. Comprehensive data preprocessing and feature engineering
2. Multiple regression algorithms including Linear Regression, Decision Tree, Random Forest, and Boosting Algorithms.
3. Deployment setup for AWS using CI/CD pipelines.


# Components

1. Data Ingestion is apart of components module which means reading dataset from databases/file locations

2. Ingested data is transformed inside data_transformation.py

3. Model Training will happen in model_trainer.py

4. Model prediction is occuring in predict_pipeline.py

5. Logger has all the log files

6. Exception handling is taking care by exception.py, exc_info() tells the file name and line number where the exception is occuring


# AWS Deployment

1. Utilization of AWS services like IAM, ECR, and EC2.
2. Docker setup on AWS EC2 for container management.
3. GitHub Actions for CI/CD.


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

Run the commands shown after the runner is created in GitHub for Downloading, Configuring and Running the self-hosted runner


# Setup github secrets:

AWS_ACCESS_KEY_ID=

AWS_SECRET_ACCESS_KEY=

AWS_REGION = us-east-1

AWS_ECR_LOGIN_URI = demo>> 566373416292.dkr.ecr.ap-south-1.amazonaws.com

ECR_REPOSITORY_NAME = simple-app



# Contributing

Contributions to this project are welcome. Please fork the repository and submit a pull request.
