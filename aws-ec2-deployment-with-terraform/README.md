# AWS EC2 Deployment with Terraform

## Overview
This project demonstrates provisioning an Amazon EC2 instance inside a custom VPC using Terraform. It dynamically fetches the latest Amazon Linux 2 AMI ID and sets up required networking components such as VPC, subnet, and security groups.

## Project Highlights
- Infrastructure as Code (IaC) using Terraform  
- Dynamic AMI ID fetching for up-to-date EC2 images  
- Custom VPC and subnet configuration  
- Security group setup allowing SSH access  
- Modular, reusable, and well-commented Terraform code  

## Technologies Used
- **Terraform** for infrastructure provisioning  
- **AWS EC2, VPC, Subnet, Security Groups**  

## How To Deploy

## How to Deploy

1. **Clone the repository**
   ```bash
   git clone https://github.com/Prafful-018/DevOps-Project.git
   cd DevOps-Project/aws-ec2-deployment-with-terraform

2.Initialize Terraform
```bash
terraform init

3.Review the plan
```bash
terraform plan

4.Apply the configuration
```bash
terraform apply

5.Confirm the deployment
```bash
Terraform will output the public IP of the EC2 instance after successful apply.

6.Connect to EC2 instance
```bash
ssh -i your-key.pem ec2-user@<EC2-Public-IP>

7.Tear down resources (Optional)
```bash
terraform destroy





