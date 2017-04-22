***Linux-Server-Configuration-UDACITY***

In this project, a Linux virtual machine needs to be configurated to support the Item Catalog website. I have used Amazon Light sail to create a virtual machine and deploy catalog app

You can visit http://34.207.168.240/ to check the deployed app.

Project Overview

A baseline installation of a Linux distribution on a virtual machine and prepare it to host web applications, to include installing updates, securing it from a number of attack vectors and installing/configuring web and database servers

> Why this Project?

>> A deep understanding of exactly what web applications are doing, how they are hosted, and the interactions between multiple systems are. This project, turns a brand-new, bare bones, Linux server into the secure and efficient web application host that a Data Driven Web Applications Needs.

> Major Keypoints

>> i.Deploying a web application to a publicly accessible server.
>> ii.Properly securing application ensures, application remains stable and that user’s data is safe.

Tasks

1. Launch your Virtual Machine with your Udacity account
2. Follow the instructions provided to SSH into your server
3. Create a new user named grader
4. Give the grader the permission to sudo
5. Update all currently installed packages
6. Change the SSH port from 22 to 2200
7. Configure the Uncomplicated Firewall (UFW) to only allow incoming connections for SSH (port 2200), HTTP (port 80), and NTP (port 123)
8. Configure the local timezone to UTC
9. Install and configure Apache to serve a Python mod_wsgi application
10. Install and configure PostgreSQL:
11. Do not allow remote connections
12. Create a new user named catalog that has limited permissions to your catalog application database
13. Install git, clone and setup your Catalog App project (from your GitHub repository from earlier in the Nanodegree program) so that it functions correctly when visiting your server’s IP address in a browser. Remember to set this up appropriately so that your .git directory is not publicly accessible via a browser!
14. Launch Virtual Machine

***Instructions for SSH access to the instance***

Download Private Key from Amazon Light sail account page below

Move the private key file into the folder ~/.ssh (where ~ is your environment's home directory). So if you downloaded the file to the Downloads folder, just execute the following command in your terminal. mv ~/Downloads/LightsailDefaultPrivateKey.pem ~/.ssh/

Open your terminal and type in chmod 600 ~/.ssh/LightsailDefaultPrivateKey.pem
In your terminal, type in ssh -i ~/.ssh/LightsailDefaultPrivateKey.pem root@34.207.168.240

Development Environment Information

Public IP Address
34.207.168.240
