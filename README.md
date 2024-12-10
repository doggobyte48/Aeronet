# Aeronet
The source of the Aeronet project, a proxy server that recreates the 2010 internet.
## Requirements
A Linux computer with Ubuntu or any other distro based on Debian
## How to Install
To get your own Aeronet server running you will have to install SquidProxy and Apache2 with the following commands

`sudo apt install squid`

`sudo apt install apache2`

**DO NOT RUN THE SERVICES YET**

Instead you need to copy first squid.conf to  `etc/squid/` 
and overwrite the the pre-existing config then you can start the services with the following command

`sudo systemctl start apache2`

`sudo systemctl start squid`
