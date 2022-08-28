# Servian_test
This is for deploying containerized app in ECS using Terraform

# Pre-requisites:
    1 Terraform installed
    2 An AWS account
    3 A properly configured AWS account on your local environment
    4 Docker installed.

# Steps

# Clone Github project.
    git clone https://github.com/RanjitRajput/Servian_test.git

# Using IAC tool Terraform to Deploy AWS service and ECS Cluster.
    terraform init
    terraform plan
    terraform apply

# Login to AWS console --> ECS---> Verify ECS Cluster status.

# CICD

We can Use Jenkins pipeline as CICD tool to automate way of deployment.
After the CI/CD Docker Pipeline is successfully set up, we will push commits to our GitHub repository and in turn, GitHub Webhook will trigger the CI/CD Pipeline on Jenkins Server. Jenkins Server will then pull the latest code, carry out unit tests, build a docker image and push it to AWS ECR. After the image is pushed to AWS ECR, the same image will be deployed in AWS ECS by Jenkins.

