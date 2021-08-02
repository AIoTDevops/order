

## centos
 sudo yum install -y yum-utils
 sudo yum-config-manager \
    --add-repo \
    https://download.docker.com/linux/centos/docker-ce.repo


 sudo yum install docker-ce docker-ce-cli containerd.io


 sudo systemctl start docker


 sudo docker run hello-world




## docker-compose

sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose


sudo chmod +x /usr/local/bin/docker-compose


docker-compose --version


## docker external network
docker network create es_network



## mysql

CREATE DATABASE db_name;

## web页面
hadoop namenode 50070


## 删除

- You can delete the lock file with the following command:

sudo rm /var/lib/apt/lists/lock


- You may also need to delete the lock file in the cache directory

sudo rm /var/cache/apt/archives/lock
sudo rm /var/lib/dpkg/lock




```
sudo rm /var/lib/dpkg/lock-frontend


sudo rm /var/lib/apt/lists/lock
sudo rm /var/cache/apt/archives/lock
sudo rm /var/lib/dpkg/lock
```





## 进程
ps aux | grep [a]pt


pgrep -a apt


sudo kill -9 processnumber





## centos ssh
1. aws   sudo passwd 
2. vi /etc/ssh/sshd_config
3. PermitRootLogin yes
4. PasswordAuthentication yes
5. vi /root/.ssh/authorized_keys
6. systemctl restart sshd    /etc/init.d/sshd restart


ifconfig

netstat -anp | grep :22

service sshd start 
service iptables stop



## ubuntu 18.04

apt-get update
apt-get install docker.io

docker --version
docker pull hello-world
docker run hello-world

service docker restart

docker ps -a


docker compose


sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose



sudo chmod +x /usr/local/bin/docker-compose


apt-get install docker-compose

sudo ln -s  /usr/bin/docker-compose  /usr/local/bin/docker-compose
