Project Overview: Coworking Space Service
The Coworking Space Service is a set of APIs that enables users to request one-time tokens and administrators to authorize access to a coworking space. This service follows a microservice pattern and the APIs are split into distinct services that can be deployed and managed independently of one another. For this project, you are a DevOps engineer who will be collaborating with a team that is building an API for business analysts. The API provides business analysts with basic analytics data on user activity in the coworking space service. The application they provide you functions as expected, and you will help build a pipeline to deploy it to Kubernetes. You'll submit artefacts from the build and deployment of this service.

Step 1: Set Up a Postgres Database with Helm Chart
Pre-requisites:

Have Kubernetes cluster ready.
Have kubectl installed and configured to interact with your cluster.
Have Github account
Fork and Clone Project Repoository
Instructions: Docker: An open-source platform for containerization, Docker enables us to package microservices into lightweight, portable containers that can run consistently across different environments.

Docker CLI: The Docker command-line interface (CLI) allows us to interact with Docker, build images, and manage containers.

Python 3: A versatile and widely-used programming language, Python 3 will be used to create microservices and scripts throughout the course.

Python PIP: The Python Package Installer (PIP) is a tool for installing and managing Python packages, which we'll use to manage dependencies for our microservices.

AWS CLI: The AWS Command Line Interface (CLI) is a unified tool to manage AWS services, enabling us to interact with AWS resources directly from the command line.

AWS CodeBuild: A fully managed continuous integration service, AWS CodeBuild will be used to build, test, and package our microservices' source code.

AWS Elastic Kubernetes Service (EKS): A managed Kubernetes service, AWS EKS will help us deploy, manage, and scale containerized applications using Kubernetes.

AWS Elastic Container Registry (ECR): A fully managed Docker container registry, AWS ECR allows us to store, manage, and deploy Docker container images.

AWS CloudWatch: A monitoring and observability service, AWS CloudWatch will help us collect and analyze logs, metrics, and events from our Kubernetes clusters and microservices.

kubectl: The Kubernetes command-line tool, kubectl, allows us to run commands and interact with Kubernetes clusters.

Helm: A package manager for Kubernetes, Helm enables us to manage, deploy, and upgrade Kubernetes applications using charts that define application configurations.

git CLI: The Git command-line interface allows us to interact with Git repositories, perform version control operations, and collaborate on code development.

GitHub: A web-based platform for version control and collaboration, GitHub will be used to host our code repositories and facilitate collaboration on our microservices.

Create a Dockerfile for the Python Application
Dockerfile Pls find the file under the root directory

Write a Build Pipeline with AWS CodeBuild
buildspec File Pls find the file under the root directory

BulidCode history Please refer the screen print in the attached document under Project-Screenprints directory.

Create Kubernetes Service and Deployment
List Services

kubectl get svc
kubectl describe svc
List Pods

kubectl get pods
kubectl describe pods
List Pods Please refer the screen print in the attached document under Project-Screenprints directory. List Describe Pods DB Please refer the screen print in the attached document under Project-Screenprints directory. List Describe Pods API Please refer the screen print in the attached document under Project-Screenprints directory.

List Deployments

kubectl get deployments
kubectl describe deployment coworking
List Deployments Please refer the screen print in the attached document under Project-Screenprints directory. List Describe Deployments Please refer the screen print in the attached document under Project-Screenprints directory.

AWS CloudWatch for Logs
CloudWatch Logs Please refer the screen print in the attached document under Project-Screenprints directory.
Repo - https://github.com/kultarsinghportal/coworking-space
