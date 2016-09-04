# use the lastest ubuntu image
FROM ubuntu:12.04

# MAINTAINER: Dang Van Luan "bizongcntt1990@gmail.com"

# make sure the package repository is up to date
RUN echo "deb http://archive.ubuntu.com/ubuntu precise main universe" > /etc/apt/sources.list
RUN apt-get update

# install apache, mysql, php, emacs, wget and wordpress
RUN apt-get install -y mysql-server mysql-client

RUN apt-get install -y apache2 apache2-mpm-prefork apache2-utils apache2.2-common libstorable-perl libapache2-mod-php5 libapr1 libaprutil1 libdbd-mysql-perl libdbi-perl libnet-daemon-perl libplrpc-perl libpq5 mysql-common php5-common php5-mysql

RUN apt-get install -y emacs23 wget

# download the lastest version of wordpress and move the source to default apache server host /var/www
RUN wget http://wordpress.org/latest.tar.gz && mv latest.tar.gz /var/www

# setting ports to be publicly exposed when running the image
EXPOSE 80
