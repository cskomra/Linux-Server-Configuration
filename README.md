# FSND P5 Linux Server Configuration

- IP Address: 	52.89.83.65
- URL:			http://ec2-52-89-83-65.us-west-2.compute.amazonaws.com

## Summary of Software Installed
- apache2
- python-setuptools libapache2-mod-wsgi
- git
- libapache2-mod-wsgi python-dev
- python-pip
- virtualenv
- Flask
- httplib2
- requests
- flask-seasurf
- oauth2client
- sqlalchemy
- python-psycopg2
- postgresql

## Summary of Configurations Made
- disabled root user remote login 
- created remote user 'grader' with sudo access
- disabled password authentication
- changed SSH port to 2200
- only allow incoming connections:
	- SSH on port 2200
	- HTTP on port 80
	- NTP on port 123
- set local timezone to UTC
- set Apache to serve Python mod_wsgi application
- set git user name and email	
- enable Apache to serve Flask applications
- enable new virtual host on port 80
- configure wsgi
- make GitHub repo inaccessible
- configure PostgreSQL
	- no remote connections allowed
	- set create_engine to 'postgresql'
	- create default user with password
	- configure default user roles
	- create database schema
- configure Google+ OAuth
- configure Facebook OAuth	


## Third-party Resources Used
- [stuken's Linux Configuration Project](https://github.com/stueken/FSND-P5_Linux-Server-Configuration)
- [Udacity Discussion Forum](https://discussions.udacity.com/t/fix-oauth2credentials-object-is-not-json-serializable/15515)
- [Udacity / ud330 Issue #4](https://github.com/udacity/ud330/issues/4) and [Stack Overflow](http://stackoverflow.com/questions/22915461/google-login-server-side-flow-storing-credentials-python-examples)