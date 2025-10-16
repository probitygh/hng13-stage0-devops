# HNG13 DevOps Stage 0 Task #

**Name:** Emmanuel Awoke  
**Slack Display Name:** @BEE 

**Project Description:**

This repository contains my submission for the HNG13 Stage 0 DevOps Challenge.
The task involves deploying a live NGINX web server on AWS, hosting a custom HTML page, and managing a well-documented GitHub workflow all to simulate real-world DevOps deployment practices.

**Server IP/Domain:** http://52.200.10.86

**AWS EC2 Deployment**

Launched a Ubuntu 22.04 LTS EC2 instance

Allowed inbound ports:

22 (SSH)

80 (HTTP)

Connect via SSH

**Install and Configure NGINX**
`sudo apt update`
`sudo apt install nginx -y`
`sudo systemctl start nginx`
`sudo systemctl enable nginx`


**Customize Webpage**

Edit the default NGINX HTML file:
`sudo nano /var/www/html/index.html`

**Paste edited Html code**

To Save → Ctrl + O, Enter → Ctrl + X

Then confirm in your browser:
👉 http://<your-ec2-public-ip>


**🧾 Summary**

This project demonstrates practical DevOps fundamentals — using AWS EC2 to host a live web server, managing source control with GitHub, and documenting every deployment step clearly and professionally.