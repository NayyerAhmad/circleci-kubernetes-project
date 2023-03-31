# Introduction

This is a simple Node.js application that demonstrates how to use Kubernetes and CircleCI to deploy a containerized application to the cloud.

## Prerequisites

- Node.js
- Docker
- Minikube

## Installation

1. Clone the repository from Github.

2. Open the terminal and navigate to the main directory of the project.

3. Run the command "npm install" to install the necessary dependencies.

## Usage

1. Start Minikube with the command "minikube start"
2. Start the Kubernetes dashboard with the command "minikube dashboard"
3. Build the Docker image: "docker build -t <my-app>"
4. Deploy the application to Kubernetes: "kubectl apply -f kubernetes/deployment.yaml"
5. Expose the application: "kubectl expose deployment my-app --type=NodePort --port=3000"
6. Get the URL of the exposed service: "minikube service my-app --url"
7. To run the application locally without Kubernetes: "npm start"