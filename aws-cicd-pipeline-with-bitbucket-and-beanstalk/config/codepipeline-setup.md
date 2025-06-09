# 🚀 AWS CodePipeline + CodeBuild + Bitbucket
This file explains the full CI/CD configuration using Bitbucket as source and deploying via CodePipeline & Beanstalk.




## ✅ Code Commit Setup
1. **Migrated code from GitHub to Bitbucket**
2. **Created SSH key pair**
   - Verified with:
     ```bash
     ssh -T git@bitbucket.org
     ```
3. **Connected Bitbucket to AWS CodeBuild**

---
## ✅ CodeBuild Setup

1. Created CodeBuild project
2. Configured **buildspec.yml**:
   ```yaml
   version: 0.2
   phases:
     install:
       commands:
         - echo Installing dependencies
     build:
       commands:
         - echo Building app
         - zip -r app.zip *
   artifacts:
     files:
       - app.zip


## 🔐 Notes
Used S3 as artifact location
## ✅ CodePipeline Setup
Source: Bitbucket

Build: CodeBuild project

Deploy: Elastic Beanstalk

Added IAM permissions to AWSCodePipelineServiceRole
## ✅ Final Result

Code pushed to Bitbucket triggers pipeline

CodeBuild packages and uploads to S3

Beanstalk auto-updates and hosts new version

Site becomes live instantly
## 📬 Contact
Prafful Mishra

🔗 LinkedIn(www.linkedin.com/in/prafful-mishra)

💻 GitHub(https://github.com/Prafful-018/DevOps-Project)
