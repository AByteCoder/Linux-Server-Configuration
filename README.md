# Linux-Server-Configuration
Final project for udacity full stack developer nano degree. In this project we are using Amazon Web Services LightSail Service for the project deployment.
Have deployed Item-Catalog flask application as an WSGI with Apache Server.

#### Prerequisite for this project
Create an Entry in /etc/hosts
``` 35.154.31.209 www.itemcatalog.com ``` in the local machine.
** Note this step is important **

#### Things needed to Access the Server
- IP Address of the server **35.154.31.209** and ssh port **2200**.
- Complete url will be [http://www.itemcatalog.com](http://www.itemcatalog.com).
- UserName grader
- ssh keys for server is located in /home/grader/.ssh

#### Things configured in server
1. upgraded software to latest version.
1. upgraded python and pip.
1. Installed dependency needed for item-catalog project.
1. Installed Apache2.
1. installed mod-WSGI for python3.
1. Application present in ```/var/www/Flask/Flask ```
1. Configured firewall and lightsail to allow connections in port **2200** for **SSH**, **80** for **HTTP** and **123** for **NTP**.
1. Installed **Postgresql**
  - Created User **catalog**
  - created database **catalog**
1. Created **grader** User
1. Gave sudo Access to User
1. Generated SSH keys
1. Did setup SSH access and forced SSH.
1. Configured item-catalog to run on Postgresql from the initial SQLite.
1. Used stackoverflow to find the fix for google authentication problem i.e IP address doesn't work ( target error ) only text like localhost.
