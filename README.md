# EKS-Deployment-Automation

### We are using Terraform for the Infrastructure Automation for EKS and Ansible for the Application Deployment.

### vpc. tf
## Our EKS-Cluster needs a vpc where EKS worker nodes are present, The worker nodes acts as the EC2 Instances.

### eks.tf
## The eks.tf file contains all the code required for the configuration of EKS-Cluster.

### eks_worker.tf
## This file contains the Configuration for provisioning the EKS worker group needed to schedule the Kubernetes pods.

### Using Terraform we underlying the Infrastructure needed to run our application.
### Now, for the Deployment of application on my provisioned EKS-Cluster we use Ansible.


### deploy.yml
## This code uses an ansible module that runs shell commands. It has a ansible file to execute the kubectl commands to make the kubernetes changes.

### user-service.yml
## This file defines my Kubernetes service for my user service microservice.

### deployment.yml
## This file is for Kubernetes deployment.

