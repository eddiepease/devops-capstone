# Udacity DevOps Capstone Project

This repository was created as the capstone project for the Udacity Cloud DevOps course. It creates an API on AWS which generates a company vector embedding given a company name - many machine learning use cases in business required company embeddings. See below for further information.
 

## Getting started

To get the API up and running, follow the steps below:


* Run `git clone https://github.com/eddiepease/company2vec-api` on local machine
* Setup a Bing API on Azure and replace the subscription key in `urls.py`
* Setup an AWS account and replace AWS account details variables in `Jenkinsfile`
* Setup a jenkins server, installing eksctl, docker and all dependencies in `requirements.txt`. Also add AWS credentials

## Features

Vector embeddings are often used for natural language processing in machine learning. They are used to represent a 
concept as a vector - this vector can then be used in a machine learning model. The embedding is created though a 
combination of an Azure API (to find the company website), scrapy (to do a shallow scrape of the company website) and
pre-trained GloVe embeddings.

The API is deployed, via a Jenkins CI/CD pipeline, onto EKS in AWS.


## Licensing

This project is licensed under [MIT License](https://opensource.org/licenses/MIT).

[issues]:https://github.com/jehna/readme-best-practices/issues/new
