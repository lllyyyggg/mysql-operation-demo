数据库的备份

```
mysqldump -h 218.77.105.241 -P 33306 -u root -p jc_common_db > ~/Desktop/jc_quality_db.sql
```

数据库的还原

```
mysql -h 218.77.105.241 -P 33306 -u root -p jc_quality_db < ~/Desktop/jc_quality_db.sql
```

