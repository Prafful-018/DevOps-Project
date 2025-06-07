#  AWS EC2 Deployment with Terraform

This project demonstrates how to provision a secure, highly configurable Amazon EC2 instance inside a custom VPC using **Terraform**. It includes dynamic AMI fetching, networking resources like subnets and security groups, and infrastructure best practices.


## 📌 Project Highlights
✅ Infrastructure as Code with Terraform  
- 🔁 Dynamic AMI ID resolution  
- 🌐 Custom VPC, public subnet, and internet gateway setup  
- 🔐 Security group allowing SSH access  
- 🔄 Reusable, modular, and readable code structure  

## 🧰 Tech Stack
- **Provisioning:** Terraform  
- **Cloud Platform:** AWS (EC2, VPC, Subnet, IGW, SG)  
- **OS Image:** Ubuntu Server 24.04 LTS  
## 🚀 How to Deploy This Project
### ✅ Prerequisites

- AWS Account + IAM user with programmatic access  
- AWS CLI configured locally (`aws configure`)  
- Terraform installed (`terraform -v`)  
- SSH key pair to access EC2  

### 🛠️ Steps to Deploy

1. **Clone the repository**
   ```bash
   git clone https://github.com/Prafful-018/DevOps-Project.git
   cd DevOps-Project/aws-ec2-deployment-with-terraform

2. **Initialize Terraform**
   ```bash
   terraform init

3. **Preview planned resources**
   ```bash
   terraform plan

4. **Deploy infrastructure**
   ```bash
   terraform apply

5. **Get EC2 public IP and connect**
   ```bash  
  ssh -i your-key.pem ec2-user@<EC2_PUBLIC_IP>

6. **Tear down resources (Optional)**
   ```bash
   terraform destroy
## Architecture diagram
![image](https://github.com/user-attachments/assets/7bf057ec-2818-4880-b862-e56e56e8f0bd)



🧠 **Learning Objectives**

This project is perfect to showcase:

-Understanding of Terraform basics and best practices

-Real-world cloud infrastructure provisioning on AWS

-Networking concepts like CIDR, subnets, and security groups

-Reusability and collaboration through open-source repo


## 📬 Contact
Prafful Mishra

🔗 LinkedIn(www.linkedin.com/in/prafful-mishra)

💻 GitHub(https://github.com/Prafful-018/DevOps-Project)





