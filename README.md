数据库的备份

```
mysqldump -h host -P port -u root -p jc_common_db > ~/Desktop/jc_quality_db.sql
```

数据库的还原

```
mysql -h host -P port -u root -p jc_quality_db < ~/Desktop/jc_quality_db.sql
```

