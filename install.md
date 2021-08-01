


## 常用命令
1. netstat -anp | grep :22     mac 端口   lsof -i:8080
2. ps -ef | grep mysql
3. 环境变量 /etc/profile






## centos ssh
1. aws   sudo passwd 
2. vi /etc/ssh/sshd_config
3. PermitRootLogin yes
4. PasswordAuthentication yes
5. vi /root/.ssh/authorized_keys
6. systemctl start sshd    /etc/init.d/sshd restart


ifconfig

netstat -anp | grep :22

service sshd start 
service iptables stop



##  java

yum install java



## git
yum install git



git config --global user.name "sun"
git config --global user.email "sun@1.com"

ssh-keygen -t rsa -C "sun@1.com"




## maven

bin.zip   wget 

unzip 

vim /etc/profile
export MAVEN_HOME= 
export PATH=$MAVEN_HOME/bin:$PATH


. /etc/profile


## Tomcat
  


binary distribution   zip  wget
unzip
chmod a+x -R *      mac: chmod 755 *.sh
vim conf/server.xml

bin/startup.sh

ps -ef | grep tomcat


## mysql
   wget https://dev.mysql.com/get/mysql57-community-release-el7-11.noarch.rpm
   rpm -Uvh mysql57-community-release-el7-11.noarch.rpm

   yum install mysql-community-server

   systemctl start mysqld.service

   grep 'temporary password' /var/log/mysqld.log


   mysql -uroot -p

   ALTER USER 'root'@'localhost' IDENTIFIED BY '261500Aa!';

   GRANT ALL PRIVILEGES ON *.* TO 'root'@'%' IDENTIFIED BY '261500Aa!' WITH GRANT OPTION;

   FLUSH PRIVILEGES;
   
## jdbc

5. jdbc   useSSL=false"
   


## jenkins

1. jenkins.io .war  weget
2. java -jar jenkins.war 8080