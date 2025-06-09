# 🏗️ AWS Elastic Beanstalk Setup

This file documents the setup process for hosting the vProfile application using AWS Elastic Beanstalk (Tomcat environment).


## ✅ Steps Followed
1. **Selected Platform**: Tomcat (Java)

2. **Created Beanstalk Environment**:
   - Configured in a **custom VPC**
   - Selected **public/private subnets** for better control
   - Chose appropriate **instance type** (e.g., t2.micro)
3. **Configured Security Group**:
   - Allowed HTTP (80), HTTPS (443), and MySQL (3306) for RDS connectivity
4. **Created IAM Role for Beanstalk**:
   - Attached policies for S3, EC2, RDS, and CodePipeline
5. **Uploaded Application Code**
   - Connected to deployment pipeline via AWS CodePipeline
6. **Rolling Update & Health Monitoring**
   - Enabled rolling updates
   - Verified application health from Beanstalk dashboard

## 🔐 Key Features
- Custom VPC & Subnets
- IAM Role with least privileges
- Auto Scaling configuration
- Logs sent to CloudWatch
## 📬 Contact
Prafful Mishra

🔗 LinkedIn(www.linkedin.com/in/prafful-mishra)

💻 GitHub(https://github.com/Prafful-018/DevOps-Project)
