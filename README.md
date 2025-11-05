# 🌐 Static-Website-Deployment-on-AWS-with-Custom-Domain-HTTPS

This project demonstrates hosting a static website on an Ubuntu Linux server using Nginx, secured with HTTPS, and mapped to a custom domain using AWS Route 53 DNS.

# 📌 Status: ✅ Successfully deployed & publicly accessible

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 🚀 Project Scope / What I Completed

<img width="519" height="171" alt="image" src="https://github.com/user-attachments/assets/e4c867d7-8bc2-4591-b22e-ca24ecb002a3" />

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 📍 Step-By-Step Implementation

# 1️⃣ Create a Server on AWS EC2

  1) Launch an Ubuntu EC2 instance
  2) Open required Ports in the Security Group
     A) 80 (HTTP)
     B) 443 (HTTPS)
     C) 22 (SSH)
  3) Connect to the server using SSH

# 2️⃣ Install & Configure Nginx Web Server

    sudo apt update
    sudo apt install nginx -y
    sudo systemctl start nginx
    sudo systemctl enable nginx

# Place your website files in:   

    /var/www/html/

# 3️⃣ Purchase & Configure Custom Domain (Hosting Provider)

  1) Domain bought from Hostinger
  2) DNS Management initially on Hosting
  3) Added records provided by Route 53 ✅ (Hosting Section added as requested)

# 4️⃣ Configure AWS Route 53 DNS

  Created a Hosted Zone for the domain
  Added:
  ✅ A Record → Public IP of EC2
  ✅ CNAME Record → For www redirection

# 📌 These Route 53 records were copied and added to the Hosting Provider DNS
➡ enables the domain to resolve correctly to the AWS server ✅




