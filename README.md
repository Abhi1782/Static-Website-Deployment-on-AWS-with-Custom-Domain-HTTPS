# 🌐 Static-Website-Deployment-on-AWS-with-Custom-Domain-HTTPS

This project demonstrates hosting a static website on an Ubuntu Linux server using Nginx, secured with HTTPS, and mapped to a custom domain using AWS Route 53 DNS.

# 📌 Status: ✅ Successfully deployed & publicly accessible

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 🚀 Project Scope / What I Completed

<img width="519" height="171" alt="image" src="https://github.com/user-attachments/assets/e4c867d7-8bc2-4591-b22e-ca24ecb002a3" />

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 📍 Step-By-Step Implementation

# 1️⃣ Create a Server on AWS EC2

  1) Launch an Ubuntu EC2 instance
  2) Open required Ports in the Security Group
     A) 80 (HTTP)
     B) 443 (HTTPS)
     C) 22 (SSH)
  3) Connect to the server using SSH

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<img width="1920" height="1030" alt="Screenshot (475)" src="https://github.com/user-attachments/assets/169cd3be-f5f1-48b2-9370-5c44635d8eb4" />

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<img width="1920" height="1022" alt="Screenshot (476)" src="https://github.com/user-attachments/assets/12041b39-d6a2-4c26-a750-0ebcf84f96e4" />

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 2️⃣ Install & Configure Nginx Web Server

    sudo apt update
    sudo apt install nginx -y
    sudo systemctl start nginx
    sudo systemctl enable nginx

## Place your website files in:   

    /var/www/html/

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<img width="1920" height="1019" alt="Screenshot (477)" src="https://github.com/user-attachments/assets/daea48dd-3af6-4e2b-8ef4-7b9b2c505a3f" />

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 3️⃣ Purchase & Configure Custom Domain (Hosting Provider)

   1) Domain bought from Hostinger
   2) DNS Management initially on Hosting
   3) Added records provided by Route 53 ✅ (Hosting Section added as requested)

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<img width="1920" height="1080" alt="Screenshot (485)" src="https://github.com/user-attachments/assets/706d674a-c14a-4c02-a35c-2c1347080d23" />

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 4️⃣ Configure AWS Route 53 DNS

  Created a Hosted Zone for the domain
  Added:
  ✅ A Record → Public IP of EC2
  ✅ CNAME Record → For www redirection

## 📌 These Route 53 records were copied and added to the Hosting Provider DNS
➡ enables the domain to resolve correctly to the AWS server ✅

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<img width="1920" height="1023" alt="Screenshot (479)" src="https://github.com/user-attachments/assets/c4c90942-bcb3-4bb9-94d2-c33877b2a49c" />

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<img width="1920" height="1080" alt="Screenshot (482)" src="https://github.com/user-attachments/assets/01ff09ca-73b5-4933-a423-ed0a720d23b1" />

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<img width="1920" height="1080" alt="Screenshot (483)" src="https://github.com/user-attachments/assets/0deef639-9284-403e-b863-cce9cb1593d9" />

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 5️⃣ Enable SSL using Certbot + Let’s Encrypt

    sudo apt install certbot python3-certbot-nginx -y
    sudo certbot --nginx -d cloudtechlearner.online -d www.cloudtechlearner.online

   1) Auto-configured Nginx for HTTPS
   2) Auto-renewal enabled

   Verify renewal:

    sudo certbot renew --dry-run

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<img width="1200" height="631" alt="Certbot" src="https://github.com/user-attachments/assets/2bbd599e-4df2-4341-9c5a-e006920fe6c2" />

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 ✅ Website now fully secure via HTTPS

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
<img width="1024" height="1024" alt="ChatGPT Image Nov 5, 2025, 08_13_59 PM" src="https://github.com/user-attachments/assets/8ed86728-59a3-4a79-aada-d6660dfd50ac" />

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

 # ✅ Final Output

     ✔ Static website is fully live, secured, and accessible globally
     ✔ Domain cloudtechlearner.online successfully mapped to AWS
     ✔ SSL certificate installed (HTTPS 🔐)
     ✔ Performance & reliability ensured with AWS infrastructure
     ✔ Hosting integration completed — DNS records from Route 53 placed in the hosting provider for domain resolution

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 <img width="1920" height="1015" alt="Screenshot (488)" src="https://github.com/user-attachments/assets/bbf64f18-aafa-4cad-b220-c3350b400e9c" />

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 📌 Tech Stack Used

<img width="386" height="169" alt="image" src="https://github.com/user-attachments/assets/c7fe12df-5593-4476-bff5-b046ca94f650" />

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 🏁 Conclusion

This project demonstrates:
  1) How to deploy a secure static website
  2) How to attach a custom domain
  3) How to use AWS Route 53 + Hosting DNS
  4) How to secure a server with HTTPS + Firewall

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# ⭐ Final Result Statement

✅ “Project Successfully Completed — A secure, production-ready static website deployed on AWS with custom domain & SSL, demonstrating real-world cloud hosting skills.”
 
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 🎉 Thank You!

## ✨ Thank you for exploring this project!

This deployment marks the successful completion of my Static Website Hosting on AWS (Ubuntu + Nginx + Route 53 + SSL) — demonstrating real-world cloud implementation, DNS           configuration, and website security using HTTPS.

## 🌍 I learned a lot about web hosting, domain mapping, and SSL encryption — and this project helped me strengthen my practical AWS cloud skills.

### 💡 Continuous learning never stops — new projects are on the way! 🚀

