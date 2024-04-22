# Kubernates Cluster Feedback Form App

# Technical Report: KubeFeedbackFormApp

## Overview:
The KubeFeedbackFormApp is a web application that allows users to provide feedback through an online form. The application consists of a responsive frontend, a backend for processing and storing form data, and a MySQL database. The application deployment is done using Kubernetes, ensuring scalability, high availability, and easy management.

## Technologies Used:
### Frontend:
- HTML
- CSS
- JavaScript (jQuery)
### Backend:
- PHP
### Database:
- MySQL
### Infrastructure:
- Kubernetes

## Implementation Details:
### Frontend:
- Developed using HTML for structuring, CSS for styling, and JavaScript (jQuery) for dynamic interactions, such as form data submission via AJAX.
### Backend:
- Implemented in PHP, with two main files:
  - conexao.php: Establishes connection with the MySQL database.
  - script.php: Receives form data sent by the frontend and inserts it into the database.
### Database:
- Uses MySQL as the database to store feedback information.
### Deployment with Kubernetes:
- Application deployment is done using Kubernetes to ensure availability, scalability, and simplified management.
- YAML configuration files are defined for frontend, backend, and MySQL deployments in both development and production environments.
- Each deployment is configured with appropriate replicas to meet expected demand in each environment.

## Deployment Procedure:
### Environment Preparation:
- Ensure a configured and functional Kubernetes cluster.
### Image Building:
- Build Docker images for the frontend and backend of the application.
### Database Configuration:
- Provision a MySQL database or use an existing one.
### Kubernetes Configuration:
- Use the provided YAML configuration files to define frontend, backend, and MySQL deployments in both development and production environments.
### Applying Manifests:
- Apply the YAML manifests to the Kubernetes cluster using the command `kubectl apply -f <file.yaml>`.
### Monitoring and Testing:
- Check if pods are running correctly using the command `kubectl get pods`.
- Test the application to ensure it is functioning as expected in both development and production environments.

## Conclusion:
The KubeFeedbackFormApp is a complete web application that allows users to provide feedback easily and efficiently. With the use of Kubernetes, the application is ready to scale according to demand and provide a reliable experience to users.
