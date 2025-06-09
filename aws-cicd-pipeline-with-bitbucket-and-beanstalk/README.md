# 🚀 AWS CI/CD Pipeline with Bitbucket, Beanstalk, RDS, and CodePipeline
This project demonstrates how to create a fully automated CI/CD pipeline using **Bitbucket as the source**, and deploying a Java (Tomcat) application to **AWS Elastic Beanstalk**, backed by **Amazon RDS**.



## ✅ What This Project Covers
- 👨‍💻 Migrated code from GitHub → Bitbucket using SSH keys
- ⚙️ Configured AWS Elastic Beanstalk (with custom VPC, IAM roles, key pairs, autoscaling)
- 🛢️ Connected Beanstalk to Amazon RDS and verified live database connectivity
- 🧪 Set up AWS CodeBuild and buildspec file to automate build
- 🚀 Built a complete AWS CodePipeline to deploy the app automatically

---
## 🧱 Folder Structure
├── app/ # vProfile application code

├── buildspec.yml # CI instructions for CodeBuild

├── config/ # Step-by-step infra config docs

├── screenshots/ # Proof images (RDS, pipeline, 
Beanstalk)

├── architecture.png # CI/CD architecture diagram

└── README.md # This file


## 🛠️ Tech Stack
- **Bitbucket** - Source repo
- **Elastic Beanstalk** - App hosting on Tomcat
- **Amazon RDS** - Backend DB (MySQL)
- **AWS CodeBuild** - App build step
- **AWS CodePipeline** - Complete CI/CD workflow
- **IAM, VPC, EC2, S3** - Supporting AWS resources

---
## 📝 Key Steps (Short Summary)
1. **Elastic Beanstalk Setup**
   - Custom VPC, subnet, key pair, IAM roles
   - Autoscaling group + rolling deployment

2. **RDS Setup**
   - Created MySQL instance
   - Installed `mysqlclient` using `.ebextensions`
   - Verified DB connection

3. **Bitbucket Migration**
   - Generated SSH key
   - Connected Bitbucket to local machine
   - Verified using `ssh -T git@bitbucket.org`

4. **CodeBuild Setup**
   - Configured buildspec.yml
   - Set up IAM roles and policies
   - Connected Bitbucket to CodeBuild

5. **CodePipeline Setup**
   - Created full pipeline with source → build → deploy stages
   - Website hosted on Beanstalk

---

## 📸 Screenshots

  ✅Pipeline

  <img width="959" alt="Deploying" src="https://github.com/user-attachments/assets/2a00cf11-f441-4fae-a0ee-34adbd9c43c5" />

---
  🚀 Beanstalk

<img width="959" alt="Checking connection of Beanstalk instance to RDS instance" src="https://github.com/user-attachments/assets/d4ab65e1-c3f0-4ed1-80d1-b6f1115773f8" />

---
  🛢️RDS 
  
<img width="959" alt="Creating RDS on aws" src="https://github.com/user-attachments/assets/20d59cc1-bdc9-48e6-8eb3-f7179ae78f70" />
<img width="959" alt="Verified the connections" src="https://github.com/user-attachments/assets/fbda37a6-c68a-448d-88cc-d1235ff02866" />




---
## 🧠 Learnings

- SSH key-based Bitbucket integration
- Beanstalk + RDS network setup
- Automating CI/CD with AWS-native tools
## 🙋‍♂️ About Me
I'm **Prafful Mishra**, a DevOps Engineer passionate about automating deployments and building reliable cloud infrastructure.  
Looking for roles in **top product-based companies** that value innovation and real-world skill-building.
## 📬 Contact
Prafful Mishra

🔗 LinkedIn(www.linkedin.com/in/prafful-mishra)

💻 GitHub(https://github.com/Prafful-018/DevOps-Project
