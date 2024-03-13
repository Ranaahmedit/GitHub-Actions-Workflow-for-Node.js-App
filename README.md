# GitHub Actions Workflow for Node.js Application on Kubernetes Cluster (EKS):

![nodejs](https://github.com/Ranaahmedit/GitHub-Actions-Workflow-for-Node.js-App/assets/127610751/b2bcf2eb-822e-4c98-ad84-6994eb5fe844)


## Introduction
GitHub Actions empowers you to automate your CI/CD pipelines directly from your GitHub repository. In this tutorial, we'll harness the power of GitHub Actions to deploy your Node.js project as a microservice on a Kubernetes cluster.

## Prerequisites

### Knowledge Prerequisites
- Basic understanding of Git and GitHub
- Familiarity with Node.js, npm, Docker, and Kubernetes concepts

### Setup Prerequisites
1. GitHub account and a repository containing your Node.js project
2. Docker Hub account for Docker image storage
3. Access to a Kubernetes cluster EKS (e.g., GKE, AKS, or self-managed)

### Tools/Technologies Used
- Git, GitHub
- Node.js, npm
- Docker
- Kubernetes

## Step-by-Step Guide

### Step 1 – Setting Up GitHub Actions Workflow for Continuous Integration (CI)
- Go to the "Actions" tab in your GitHub repository.
- Click "Set up a workflow yourself" to create a new workflow file.
- Define triggers for CI, such as pull_request events to the master branch.
- Specify jobs and steps to build and test your Node.js application.

### Step 2 – Setting Up GitHub Actions Workflow for Continuous Deployment (CD)
- Create a separate workflow file for CD, focusing on deployment steps.
- Define triggers for CD, such as push events to a deployment branch.
- Specify jobs and steps to deploy your Node.js application to Kubernetes.

### Step 3 – Building the Node.js Application
- Use Docker to build a Docker image for your Node.js app.
- Tag the Docker image with a version latest.

### Step 4 – Pushing Docker Image to Docker Hub
- Authenticate with Docker Hub using Docker credentials.
- Push the Docker image to Docker Hub for storage.

   ![cre](https://github.com/Ranaahmedit/GitHub-Actions-Workflow-for-Node.js-App/assets/127610751/1c9c1e25-c825-4cff-8237-3c565dbea5c9)


### Step 5 – Deploying to Kubernetes Cluster
- Apply Kubernetes manifests using kubectl or a similar tool.
- Create Kubernetes deployment for your Node.js app.

### Step 6 – Testing Deployment
- Verify the deployment by accessing the application endpoint.
- Perform necessary tests to ensure correct functionality.

 ### CI Workflow
   
  ![ci](https://github.com/Ranaahmedit/GitHub-Actions-Workflow-for-Node.js-App/assets/127610751/88a8feb9-d40f-46e1-a04c-fdd74888e999)


   This screenshot shows the CI workflow in action, building and testing the Node.js application.


### CD Workflow

  ![cd](https://github.com/Ranaahmedit/GitHub-Actions-Workflow-for-Node.js-App/assets/127610751/7322b2eb-e246-4378-ac03-752de3631957)

This screenshot shows the CD workflow deploying the Node.js application to Kubernetes.


## Conclusion
With this GitHub Actions workflow, automate the deployment of your Node.js app as a microservice on Kubernetes, streamlining your development and deployment process. Leverage GitHub Actions for faster, more reliable deployments while maintaining control and visibility over your CI/CD pipeline.



🚀 Happy deploying!


