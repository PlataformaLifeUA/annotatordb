# annotatordb
The MySQL database for the web annotator.

This repository contains the dump of the MySQL database with the database structure, scripts to fill it with the corpus data and other useful scripts.

1. TO INSTALL THE DATABASE

* Create a MySQL database:

```bash
echo "CREATE DATABASE annotation" | mysql -u root -p
echo "GRANT ALL PRIVILEGES ON annotation.* TO annotation@localhost IDENTIFIED BY 'annotation' | mysql -u root -p
```

This create a database called "annotation" and a user called 'annotation' with the password 'annotation' to access to the database.

  * Dump the file in the database

```bash
cat annotation.sql | mysql -u annotationusr -p'annotationpass' annotation
```

2. POPULATE THE DB WITH THE CORPUS DATA

Coming soon
