# ---------------RUN MYSQL COMMAND ON ARCH LINUX--------------

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

These are the basic steps to install MySQL on Arch Linux and run MySQL commands. Keep in mind that the specifics may vary slightly depending on the version of MySQL available in the Arch Linux repositories. Always refer to the Arch Linux documentation or MySQL documentation for the most up-to-date information.
