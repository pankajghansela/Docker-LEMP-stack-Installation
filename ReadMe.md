# This program installs the LEMP stack (Linux, Nginx, MySQL, PHP) with just one Docker command

# Please note that the NGINX service in this program is configured to listen on PORT 8059 and NOT THE DEFAULT port 80!

# Environment variabes
	
  mysql root password: admin
  
  php myadmin user: root
  php myadmin password: admin

# Error logs for the Nginx, if any, can be acccessed inside the /logs directory 

# The Docker file contains the Nginx:latest image which installs the full nginx package. This was created separately to properly install the fastcgi-fpm config, so it doesn't cause an error.

# The Docker compose creates 4 containers for: nginx, php fpm, mysql and php myadmin


To install the stack, simply clone the repository and run the command:
 "docker-compose up -d" 
from the parent directory where this ReadMe file is located 
