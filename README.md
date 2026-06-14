Step-by-step guide to deploying a web server on AWS EC2 using Free Tier

Topics: aws, ec2, webserver, linux, free-tier
Architecture
text

Internet User
│
▼
┌─────────────────────┐
│ AWS EC2 Instance │
│ (Free Tier) │
│ ┌────────────────┐ │
│ │ Apache/Nginx │ │
│ │ Web Server │ │
│ └────────────────┘ │
│ ┌────────────────┐ │
│ │ Linux (Ubuntu) │ │
│ └────────────────┘ │
│ ┌────────────────┐ │
│ │ Security Groups│ │
│ │ SSH | HTTP|HTTPS│ │
│ └────────────────┘ │
└─────────────────────┘
What You'll Learn
Launching an EC2 instance on AWS Free Tier
Configuring Security Groups (SSH, HTTP, HTTPS)
Connecting via SSH using Key Pairs
Installing and configuring Apache/Nginx web server
Setting up firewall rules (UFW)
Assigning Elastic IP for persistent access
Prerequisites
AWS Free Tier Account
Basic Linux command line knowledge
Steps
Create AWS Account — Sign up for Free Tier
Launch EC2 Instance — Select Ubuntu/Amazon Linux AMI
Configure Security Groups — Allow SSH(22), HTTP(80), HTTPS(443)
Create Key Pair — Download .pem file for SSH access
SSH into Instance — ssh -i key.pem ubuntu@
Install Web Server — sudo apt install nginx
Configure Firewall — sudo ufw allow 'Nginx Full'
Verify — Open public IP in browser
Technologies
AWS EC2 (t2.micro / t3.micro)
Amazon Linux / Ubuntu
Apache / Nginx
Security Groups & NACLs
SSH Key Pairs
Elastic IP
Cost
Free Tier eligible — $0/month for 12 months (t2.micro or t3.micro)

Author: Yeswanth P | GitHub | LinkedIn
