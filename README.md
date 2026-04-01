\# Three-Tier Architecture Deployment on AWS using Terraform



\## Project Overview



This project demonstrates the deployment of a scalable, secure, and highly available infrastructure on AWS using Terraform. It follows a three-tier architecture design pattern and leverages Infrastructure as Code (IaC) to automate resource provisioning.



\## Architecture



The architecture is designed with separation of concerns across different layers:



\* Virtual Private Cloud (VPC) with public and private subnets

\* Internet Gateway and NAT Gateway for controlled internet access

\* Security Groups for secure communication between layers

\* EC2 instances configured with Apache Web Server

\* Auto Scaling Group to ensure scalability and fault tolerance

\* Application Load Balancer (ALB) for traffic distribution



\## Technologies Used



\* Terraform (Infrastructure as Code)

\* Amazon Web Services (EC2, VPC, ALB, Auto Scaling, NAT Gateway)

\* Apache Web Server



\## Key Features



\* High availability across multiple Availability Zones

\* Automatic scaling based on demand

\* Secure network architecture using private subnets

\* Fully automated deployment using Terraform



\## Application Output



The application is accessible via the Load Balancer DNS and returns:



"Hello from Auto Scaling"



\## How to Run



```bash

terraform init

terraform apply

```



\## Cleanup



```bash

terraform destroy

```



\## Future Enhancements



\* Integrate a Node.js backend application

\* Add a relational database using Amazon RDS

\* Implement monitoring and logging using CloudWatch

\* Configure domain and HTTPS using Route 53 and SSL



