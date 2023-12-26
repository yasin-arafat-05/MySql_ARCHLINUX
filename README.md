<br>

# __________ RUN MYSQL COMMAND ON ARCH LINUX __________

<br>

### Installation:

Open a terminal and run the following command to install MySQL:

```bash
sudo pacman -S mysql
```

### Start and Enable MySQL service:

Once the installation is complete, you need to start and enable the MySQL service. Run the following commands:

```bash
sudo systemctl start mysqld
sudo systemctl enable mysqld
```

### Secure MySQL Installation:

MySQL comes with a script to secure the installation. Run the following command and follow the prompts:

```bash
sudo mysql_secure_installation
```

This script will guide you through setting a root password, removing anonymous users, disallowing root login remotely, and more.

### Access MySQL Shell:

After installation and securing, you can access the MySQL shell using the following command:

```bash
mysql -u root -p
```

You will be prompted to enter the root password you set during the secure installation.

### Running MySQL Commands:

Once you are in the MySQL shell, you can run SQL commands. For example:

```sql
SHOW DATABASES;
```
It is DATABASES not DATABASE.
This will display a list of databases.

Remember to exit the MySQL shell when you are done:

```sql
EXIT;
```

<br>

# __________How Many Users Are In MY MYSQL SERVER__________

<br>

There is a Default database name `mysql`. To check how many users are available in your server check the 
table name `user` in `mysql` database.

- Follow This command

```sql
SHOW DATABASES;
```

```sql
USE mysql;
```

```sql
SHOW TABLES;
```

```sql
DESCRIBE user;
```

```sql
SELECT user FROM user;
```
