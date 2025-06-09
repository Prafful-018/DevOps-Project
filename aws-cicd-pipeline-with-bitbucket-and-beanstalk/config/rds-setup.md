# 🛢️ Amazon RDS Setup & Beanstalk Connectivity

This file explains how RDS was created and connected with Beanstalk for backend DB integration.



## ✅ RDS Setup
1. **Created RDS Instance** (MySQL/PostgreSQL):
   - Chose DB engine: MySQL
   - Allocated storage: 20GB
   - Multi-AZ: Disabled
   - Enabled public accessibility (for testing only)

2. **Subnet Group & VPC**
   - RDS placed in same VPC as Beanstalk
   - Subnet group aligned with Beanstalk private subnet

3. **Security Groups**
   - Opened port `3306` from Beanstalk SG to RDS SG

4. **Installed `mysqlclient` on Beanstalk**:
   - Used `.ebextensions/01_packages.config`:
     ```yaml
     packages:
       yum:
         mysql: []
         python3-devel: []
         mysql-devel: []
     ```

5. **Environment Variables**
   - Added DB host, username, password in Beanstalk configuration
## ✅ Connection Verified

- SSH'd into Beanstalk instance
- Ran:
  ```bash
  mysql -h <RDS-ENDPOINT> -u admin -p

## 🔐 Notes
-Always restrict RDS access via SGs, not public IP

-Store DB credentials using AWS Secrets Manager or Beanstalk Env Vars
## 📬 Contact
Prafful Mishra

🔗 LinkedIn(www.linkedin.com/in/prafful-mishra)

💻 GitHub(https://github.com/Prafful-018/DevOps-Project)
