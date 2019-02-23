数据库的备份

```
mysqldump -h host -P port -u root -p jc_common_db > ~/Desktop/jc_quality_db.sql
```

数据库的还原

```
mysql -h host -P port -u root -p jc_quality_db < ~/Desktop/jc_quality_db.sql
```

数据库的端口号

```
sudo cat /var/run/mysqld/mysqld.pid
```

停止mysql服务

```
sudo kill port
/etc/init.d/mysqld stop
```
重新装mysql
```
find / -name mysql (rm -rf /var/lib/mysql)
rpm -qa|grep mysql (yum remove)
rm /etc/my.cnf*
rpm -qa | grep -i mysql(rpm -e MySQL-server-5.6.17-1.el6.i686)
chkconfig --list | grep -i mysql (chkconfig --del mysql)
find / -name mysql
通过上面的步骤mysql就删除完全了

rpm -ivh http://repo.mysql.com/yum/mysql-5.5-community/el/6/x86_64/mysql-community-release-el6-5.noarch.rpm
vim /etc/yum.repos.d/mysql-community.repo
yum install mysql-community-client mysql-community-devel mysql-community-server php-mysql
此处已经安装完毕
```

