# Three-Tier Architecture Deployment on AWS using Terraform

## Project Overview

This project demonstrates the deployment of a scalable and highly available infrastructure on AWS using Terraform. The focus of this project is on infrastructure provisioning, networking, and automated deployment using Infrastructure as Code (IaC).

## Architecture

The infrastructure is designed to simulate a multi-tier architecture with the following components:

* Virtual Private Cloud (VPC) with public and private subnets
* Internet Gateway for public access
* NAT Gateway for secure outbound internet access from private subnets
* Security Groups to control traffic between components
* EC2 instances configured with Apache Web Server
* Auto Scaling Group to manage multiple EC2 instances
* Application Load Balancer (ALB) to distribute incoming traffic

## Technologies Used

* Terraform (Infrastructure as Code)
* Amazon Web Services (EC2, VPC, ALB, Auto Scaling, NAT Gateway)
* Apache Web Server

## Key Features

* High availability using multiple Availability Zones
* Load balancing using Application Load Balancer
* Automatic scaling using Auto Scaling Group
* Secure network design using public and private subnets
* Fully automated infrastructure deployment

## Application Output

The application is accessible via the Load Balancer DNS and displays:

"Hello from Auto Scaling"

## Steps Performed

1. Configured AWS provider using Terraform
2. Created VPC and defined CIDR blocks
3. Created public and private subnets
4. Attached Internet Gateway to VPC
5. Configured route tables for public and private subnets
6. Created NAT Gateway for private subnet internet access
7. Defined Security Groups for controlled communication
8. Launched EC2 instance and configured Apache server
9. Created Launch Template for Auto Scaling
10. Configured Auto Scaling Group across multiple subnets
11. Created Application Load Balancer
12. Attached Target Group and Listener to ALB
13. Verified deployment using Load Balancer DNS

## How to Run

```bash
terraform init
terraform apply
```

## Cleanup

```bash
terraform destroy
```

## Notes

This project focuses on infrastructure and deployment. It can be extended in the future by adding an application backend and database layer.




## Output Screenshot

Below is the output of the deployed application accessed via the Load Balancer:



