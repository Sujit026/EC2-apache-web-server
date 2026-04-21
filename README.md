# EC2 Apache Web Server Deployment on AWS
Deploying Apache Web Server on AWS EC2

**Project Overview**  

This project demonstrates how to deploy a web server on AWS EC2 and host a static website using Apache.  

**Architecture**  

User → Internet → Internet Gateway → EC2 → Apache Web Server   

**Implementation Steps**  

**Step 1 -** Created a custom VPC, Created a Public Subnet, Configured Route Table and associated it with subnet and Attached Internet Gateway (IGW) to VPC.  

  <img width="940" height="234" alt="image" src="https://github.com/user-attachments/assets/22cd4a80-0caa-4c20-a9ec-cd16259a789a" />
  
**Step 2 -**  Launched EC2 instance (Amazon Linux AMI)  
  
  <img width="940" height="442" alt="image" src="https://github.com/user-attachments/assets/ae5cdee2-6df0-41c4-944e-8e70008560f4" />
  
  
**Step 3 -**  Created Key Pair (.pem), converted it to .ppk using PuTTYgen, and connected to EC2 via SSH using PuTTY.     

**Step 4 -**  Installed and configured Apache Web Server.  
  
  <img width="940" height="313" alt="image" src="https://github.com/user-attachments/assets/239f9be9-e5c6-4802-a668-1fd51f211c8d" />  
    
**Step 5 -** Modified default web page in `/var/www/html/index.html
  
**Output**    

Successfully hosted a custom web page accessible via EC2 public IP.
   
 <img width="754" height="259" alt="image" src="https://github.com/user-attachments/assets/78c38f7d-a920-4ca9-b158-5b4cc744b18c" />  


**Commands Used**   

sudo yum update -y        # Update packages  
sudo yum install httpd -y # Install Apache  
sudo systemctl start httpd  
sudo systemctl enable httpd  
sudo systemctl status httpd  
  
**Learnings**

- Understood VPC and public subnet configuration    
- Learned SSH connectivity using key pairs    
- Installed and managed Apache web server    
- Hosted and modified static web content    
- Gained hands-on troubleshooting experience
    
