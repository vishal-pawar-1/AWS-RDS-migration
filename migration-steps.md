# Migration Steps – MySQL Workbench to AWS RDS

---

## 1️⃣ Create AWS RDS Database
- Service: **RDS → Create Database**
- Engine: MySQL (8.x)
- Instance type: `db.t3.micro`
- Public Access: Yes
- Security group: Allow inbound port 3306
- Note down **RDS endpoint** (e.g., mydb.xxxxx.ap-south-1.rds.amazonaws.com)

---

## 2️⃣ Connect Local Database
- Open MySQL Workbench
- Connect to your **local MySQL database**

---

## 3️⃣ Connect AWS RDS Database to MySQL Workbench
- Open MySQL Workbench → Click `+` to create a **New Connection**
- Connection Name: `AWS RDS`
- Hostname: **RDS endpoint**  
- Port: `3306`
- Username: Master username (created during RDS setup)
- Password: Enter password
- Click **Test Connection** → Should say "Successfully made the MySQL connection"
- Click **OK** to save

---

## 4️⃣ Use Migration Wizard
- Navigate: `Database → Migration Wizard`
- **Source:** Local MySQL
- **Target:** AWS RDS connection
- Enter credentials if prompted
- Select schemas & tables to migrate

---

## 5️⃣ Migrate Data
- Run schema migration
- Run data migration
- Monitor logs for any errors

---

## 6️⃣ Verify Migration
- Open AWS RDS connection in Workbench
- Run:
```sql
SHOW DATABASES;
SELECT * FROM your_table;
