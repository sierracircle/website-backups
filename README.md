website-backups
================

Bash Script to backup your website files and databases

##INSTALL:

1. put the backup file into your scripts folder
2. set the options: your database user, database password, folders to backup, databases to backup
3. save your changes
4. create a cronjob (crontab -e)  and add something like one (or more) of the following:



```
#check on services
@hourly ~/.scripts/backups hourly
@monthly ~/.scripts/backup monthly
@yearly ~/.scripts/backup yearly

```

The script will get the frequency from the cronjob, and make a folder in your ~/.backups directory named after the frequency (daily, monthly, yearly)




