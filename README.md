# CE Lab: Launch EC2 Instance

**Name:** Cielo Escobar  
**Date:** 09/02/26  

## Lab Description
This lab demonstrates my first hands-on experience launching a virtual server in AWS, configuring its security, connecting via SSH, and verifying that a web server is running. The main goal was to launch an EC2 instance, set up a security group, and ensure secure access while making the instance publicly accessible for HTTP.

## Instance Details
- **Instance ID:** i-079a97faf5faecfe8  
- **Instance Type:** t3.micro  
- **Public IP:** 35.158.113.71  

## Security Group Configuration
- **Security Group ID:** sg-0e1f8043891b0f5d4  
- **Inbound Rules:**
  - SSH (TCP 22) → From my IP only
  - HTTP (TCP 80) → From anywhere (0.0.0.0/0)
- **Outbound Rules:** All traffic allowed (default)

## Screenshots
All screenshots are in the `screenshots/` folder:

1. **01-instance-running.png** – EC2 console showing running instance  
2. **02-security-group-rules.png** – Security group inbound rules  
3. **03-ssh-connection.png** – Terminal showing successful SSH connection  
4. **04-web-server-browser.png** – Web browser showing your webpage  
5. **05-instance-details.png** – Instance details page  

## Challenges & Solutions
- **Challenge:** The instance IP changed when stopping and starting it.  
  **Solution:** Updated all references to the new public IP before testing SSH and HTTP access.  
- **Challenge:** Understanding which commands to run for security verification.  
  **Solution:** Followed the lab instructions step-by-step and verified SSH, ping, and HTTP access.
