# aws-ec2-linux-web-server-project
Deployed an EC2 Linux web server with Apache and hosted a custom webpage.

# AWS EC2 Linux Web Server

## Project Overview
This project demonstrates how I launched an EC2 instance, connected to it, installed Apache, and hosted a simple webpage on a Linux server.  
This is a common task in cloud support and helped me understand how compute, networking, and web servers work together in AWS.

## Architecture
User → Browser → EC2 Public IP → Apache Web Server → HTML Page

## Services Used
- Amazon EC2  
- Security Groups  
- IAM  
- VPC Networking  

## What I Did
- Launched an EC2 instance (Amazon Linux 2)  
- Created and attached a security group allowing SSH (22) and HTTP (80)  
- Connected to the instance using SSH  
- Installed Apache (`sudo yum install httpd -y`)  
- Started and enabled the Apache service  
- Created a custom index.html file  
- Verified the webpage using the EC2 public IP  

## Example Commands Used
```bash
sudo yum update -y
sudo yum install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd
echo "<h1>Hello from Nahum's EC2 Web Server!</h1>" | sudo tee /var/www/html/index.html
```

## What I Learned
- How to launch and configure an EC2 instance  
- How security groups control inbound traffic  
- How to SSH into a Linux server  
- How to install and manage Apache  
- How to troubleshoot connection issues (security group rules, service status, etc.)  

## Skills Demonstrated
- EC2 management  
- Linux commands  
- Web server setup  
- Networking & security groups  
- Troubleshooting  

## Next Steps



# AWS EC2 Linux Web Server Project

## EC2 Instance Running
![EC2 Instance Running](screenshots/nMhVhzN3RMqVUn38u2gun.png)

## Instance Details
![Instance Details](screenshots/fVQL1rhiUVrn96kjKzm1H.png)

## Security Group Inbound Rules
![Security Group Rules](screenshots/hbcjXcypXQfAVqG5D77qb.png)

## SSH Connection
![SSH Connection](screenshots/BnCHD9it99KCWz8o9YLrc.png)

## Apache Service Running
![Apache Running](screenshots/D5pvZdCU4M8km32yEjKK1.png)

## Webpage Successfully Loaded
![Webpage Screenshot](screenshots/v25Tc3qawqewbmHkWR161.png)

- Add a custom domain using Route 53  
- Add HTTPS using an Application Load Balancer  
- Deploy a more advanced website  
- Automate setup with a user data script  
