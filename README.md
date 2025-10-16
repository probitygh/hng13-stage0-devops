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

**Paste:**

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>HNG13 DevOps Stage 0</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
      color: white;
    }
    .container {
      text-align: center;
      padding: 2rem;
      background: rgba(255, 255, 255, 0.1);
      border-radius: 10px;
      backdrop-filter: blur(10px);
    }
    h1 { margin-bottom: 1rem; }
    .timestamp { font-size: 0.9em; opacity: 0.8; }
  </style>
</head>
<body>
  <div class="container">
    <h1>Welcome to DevOps Stage 0 - Emmanuel Awoke/@BEE</h1>
    <p>Successfully Deployed on Amazon Web Services</p>
    <p class="timestamp">Deployed: 16/10/2025</p>
  </div>
</body>
</html>


To Save → Ctrl + O, Enter → Ctrl + X

Then confirm in your browser:
👉 http://<your-ec2-public-ip>


**🧾 Summary**

This project demonstrates practical DevOps fundamentals — using AWS EC2 to host a live web server, managing source control with GitHub, and documenting every deployment step clearly and professionally.