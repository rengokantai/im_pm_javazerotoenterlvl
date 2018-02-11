# im_pm_javazerotoenterlvl


### 1-5
Seperate server:
application server/ File server / Database server  

Then, not all times we need to fetch data from database server:
Distributed cache server cluster->remote distributed cache  
application->local cache

###### 08:10
Cookie with session

###### 10:27
LB->Application->data accessmodule->W(master)->R(slave)

horizonal splitting.  
Single database->single table->horizontal splitting.



### 2-1 config linux
```
wget -O /etc/yum.repos.d/CentOS.repo http://resource
yum makecache
```

###### 03:22
list:
- linux service administration. learn/537  
- iptables learn/389

### 2-3
Unistall preinstalled jdk from centos distribution
```
rpm -qa | grep jdk
rpm-ivh xxx.rpm
```
default location /usr/java
```
/usr/java/jdk1.7.0_80
```

```
vim /etc/profile
export JAVA_HOME=/usr/java/jdk1.7.0
export CLASSPATH=.:$JAVA_HOME/jre/lib/rt.jar:$JAVA_HOME/jre/lib/dt.jar:$JAVA_HOME/jre/lib/tools.jar
```
```
export PATH $JAVA_HOME/bin
source /etc/profile
```

### 3-1
```
CREATE TABLE `mmuser`(
  `id` int(11) NOT NULL AUTO_INCREMENT COMMENT 'cmt',
  `username`
  PRIMARY KEY(`id`),
  UNIQUE KEY `user_n_unique` (`username`) USING BTREE
) ENGINE=InnoDB AUTO_INCREMENT=21 DEFAULT CHARSET=utf8
```
cart.
```
CREATE TABLE `mmcart`(
`id`
`user_id`
PRIMARY_KEY(`id`),
KEY `user_id_index` (`user_id`) USING BTREE
) ENGINE=InnoDB AUTO_INCREMENT=121 DEFAULT CHARSET=utf-8
```
