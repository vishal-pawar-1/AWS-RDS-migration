# AWS RDS Database Migration Project

## 📌 Overview
This project demonstrates migrating a **local MySQL database** to **AWS RDS** using **MySQL Workbench Migration Wizard**.  
It was performed as a 2-hour demo project to showcase database migration skills.

---

## 🛠️ Tools & AWS Services Used
- AWS RDS (MySQL)
- MySQL Workbench
- IAM (for security)
- AWS Security Groups

---

## 🚀 Project Steps
1. Created AWS RDS MySQL instance with public access.
2. Configured inbound rule for port `3306` to allow local machine connection.
3. Connected **AWS RDS database to MySQL Workbench**:
   - Added a new connection using RDS endpoint, username, and password
   - Verified successful connection
4. Used **MySQL Workbench Migration Wizard**:
   - Selected local MySQL database as source
   - AWS RDS instance as target
   - Performed schema and data migration
5. Verified data on RDS by running SQL queries.
6. Documented cost estimation and screenshots.

---

## 📂 Repository Files
- `migration-steps.md` → Detailed step-by-step migration guide
- `cost-estimate.md` → Estimated AWS cost
- `screenshots/` → Images of the migration process

---

## 📊 Outcome
- Successfully migrated all tables and data.
- Ensured secure connectivity and minimal downtime.

---

## 💰 Cost
Total cost for this 2-hour demo project: **₹10 – ₹20**

---

## ✅ Skills Demonstrated
- AWS RDS Setup
- Database Migration
- IAM & Security Configuration
- MySQL Workbench

---
