
# Welcome to the README file for CLO835 Assignment 1!

By Mohd Danish Khan

## Assignment 1 Title:

## Create Dockerfile, build docker image and deploy docker container on Amazon Linux EC2  


## Table of Contents
- [Using Terraform code to Deploy EC2 instance in public subnet ](#using-terraform-to-deploy-EC2-instance-in-public-subnet)
- [Using GitHub action to create docker images and  push them to Amzon ECR](#using-github-action-for-automation)
- Using EC2 instance to host the application and database container
- Using Browser to Display the application web pages



## Using Terraform to EC2 instance in public subnet. 

Instructions on using Terraform to deploy EC2 instance.

- Clone the repo in your local machine 
 Use below command 
- git init 
- git clone https://github.com/dkhan0103/clo835-assignment.git
- Go to terraform_code/prod/instances/ directory and follow the steps 
- alias tf=terraform
- tf init # initialize terraform
- tf fmt
- tf validate
- terraform plan 
- terrform apply 


## Using GitHub action

Instructions on using GitHub action.
- Make all the application and code changes in dev branch
- Protect your main branch using branch protection
- git checkout dev 
- git add .
- git commit -m "commit "
- git push 
- Git action is triggered as follows:
- Docker workflow will trigger on any push or pull_request on master branch 

## Using EC2 instance to host the application and database container

Instruction on using EC2 instance to run docker containers
- ssh to EC2 instance 
- supply aws learner lab credentials using aws configure
- login into ecr from ec2 instance 
- Run the docker run command to build the containers on top of docker images stored in Amazon ECR

## Using Browser to Display the application web pages
Instruction
- copy the public IP of ec2 instance
- open the browser
- access http://<public ip>:8081 #for blue app
- access http://<public ip>:8082 #for pink app
- access http://<public ip>:8082 #for lime app
 




