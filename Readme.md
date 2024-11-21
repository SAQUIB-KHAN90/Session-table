# MariaDB Setup and Configuration Guide

This guide explains how to set up MariaDB, create a database, and import data from a SQL file. It also covers deployment on Amazon EC2.

## 1. Installing MariaDB

Download and install MariaDB:

```bash
sudo apt update
sudo apt install mariadb-server
```

Start MariaDB service:

```bash
sudo systemctl start mariadb
sudo systemctl enable mariadb
```

## 2. Securing MariaDB

Run the security script to configure basic security:

```bash
sudo mysql_secure_installation
```

Follow the instructions to:

Set a root password.
Remove unnecessary users and databases.
Disable remote root login.

## 3. Setting Up the Database

Log in to MariaDB:

```bash
sudo mysql -u root -p
```

Create a new database and user:

```sql
CREATE DATABASE springbackend;
GRANT ALL PRIVILEGES ON springbackend.* TO 'username'@'localhost' IDENTIFIED BY 'your_password';

```

Exit MariaDB:

```bash

EXIT;

```

## 4. Importing the Database

Import the SQL file into the database:

```bash
sudo mysql -u username -p springbackend < springbackend.sql

```

Verify the database import:

```bash

sudo mysql -u username -p

```

Run the following commands:

```bash
SHOW DATABASES;
USE springbackend;
SHOW TABLES;
SELECT * FROM tbl_workers;
```
