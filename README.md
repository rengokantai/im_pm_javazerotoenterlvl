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
