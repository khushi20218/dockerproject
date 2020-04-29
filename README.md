# Docker Project
## Description
I created my customized image which is available on docker hub.
You can find my image here. https://hub.docker.com/repository/docker/khushi09/webserver
The image consists of a web server which includes the following features:-
* httpd- for launching web server
* mysql-for creating databases
* net-tools - for basic commands like ifconfig, netstat, wget etc.
The second image that i used was a precreated image mysql:5.7 .
In this project my own webpage “myths about coronavirus” is running on top of the webserver container launched by the webserver image. This webpage consists of an input box in which the email and names are to filled . I have linked mysql database server with this container. The information about the names and the emails will automatically go and get stored in the database. This project has the issue that the IP is not dynamic and is hardcoded in the php file. 
## Pre-requisites
* linux operating system
* virtual box to host the linux operating system
* docker software inside linux
* docker compose 
## Installations
* Download the redhat linux operating system using the redhat ISO file.
* Installing docker inside the operating system
```
# cd /etc/yum.repos.d/
# gedit docker.repo
     [docker]
     baseurl=https://download.docker.com/linux/centos/7/x86_64/stable/
     gpgcgeck=0
# yum install docker-ce --nobest
```
* Installing docker compose
```
# curl -L "https://github.com/docker/compose/releases/download/1.25.4/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
# chmod +x /usr/local/bin/docker-compose
```
