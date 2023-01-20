# Installing Nginx on an Ubuntu Server on AWS

This guide will show you how to install Nginx on an Ubuntu server running on AWS.

## Connect to your Server

1. Connect to your Ubuntu server via SSH.

## Update the package lists

2. Run the following command to update the package lists:
sudo apt-get update

## Install Nginx

3. Run the following command to install Nginx:
sudo apt-get install nginx

## Verify that Nginx is running

4. Verify that Nginx is running by typing the following command:
sudo systemctl status nginx

5. You can also check if Nginx is running by visiting the server's public IP in your web browser. You should see the default Nginx welcome page.

## Configure Nginx

6. To configure Nginx, you'll need to edit the configuration files located in the `/etc/nginx` directory. The main configuration file is `/etc/nginx/nginx.conf`.

## Start, stop, or reload Nginx

7. To start, stop, or reload the Nginx server, you can use the following command:
sudo systemctl start nginx
sudo systemctl stop nginx
sudo systemctl reload nginx

8. To check for any error in configuration file use
sudo nginx -t

This will check your configuration file for any syntax errors.

That's it! You have successfully installed Nginx on your Ubuntu server on AWS. 
Please note that this guide is meant to be a basic introduction, and you might need to make additional adjustments to fit your specific needs.

Please make sure that you have proper security groups, firewall rules and also check if any ports are open or not.
