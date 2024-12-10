# Aeronet
The source of the Aeronet project, a proxy server that recreates the 2010 internet.
## Requirements
A Linux computer with Ubuntu or any other distro based on Debian
## How to Install
To get your own Aeronet server running you will have to install SquidProxy and Apache2 with the following commands

`sudo apt install squid`

`sudo apt install apache2`

**DO NOT RUN THE SERVICES YET**

Instead you need to copy first squid.conf to  `/etc/squid/` 
and overwrite the the pre-existing config.

Then you need to copy the `html` folder to `/var/www/` overwriting `var/www/html` 

Then you need to copy the `hosts` folder to `/etc` overwriting the file

Finally you need to copy the `sites-available' folder to `/etc/apache2` and enabling the virtural domains with the following command

``sudo a2ensite istart.net.conf`` 

``sudo a2ensite nintendo.com.conf`` 

Then you can start the services with the following command

`sudo systemctl start apache2`

`sudo systemctl start squid`
