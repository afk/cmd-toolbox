# MySQL

## Backup
```
# backup a single database
mysqldump -u root -p[root_password] [database_name] > dumpfilename.sql
# backup a specific table
mysqldump -u root -p[root_password] [database_name] [table_name] > dumpfilename.sql
# backup multiple databases
mysqldump -u root -p[root_password] --databases [database_name] [database_name] ... > dumpfilename.sql
# backup all databases
mysqldump -u root -p[root_password] --all-databases > dumpfilename.sql
```

## Restore
```
# restore
mysql -u root -p[root_password] [database_name] < dumpfilename.sql
```

## Backup a local database and restore to remote server
```
mysqldump -u root -p[root_password] [database_name] | mysql \
  -u root -p[root_password] --host=[remote-server] -C [database_name]
```
