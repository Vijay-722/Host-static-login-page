# **Hosting a Static Website on AWS EC2 with a Custom Domain and HTTPS Security via Certbot**


## **🧾 Project Description:**
This project involves deploying a static website on an Amazon EC2 instance, linking it to a custom domain name, and securing the connection using HTTPS with the help of Certbot and Let's Encrypt SSL certificates. It demonstrates key skills in cloud computing, web hosting, domain configuration, and SSL certificate management.


## **🛠️ Technologies Used:**
* Amazon EC2 (Amazon Linux/Ubuntu)
* Nginx (Web Server)
* Certbot (Let's Encrypt)
* Route 53 / Custom Domain Registrar (e.g., GoDaddy, Namecheap)
* SSH
* DNS Configuration (A Record, CNAME)
  

## **📦 Key Components:**
1. Static Website Deployment:
   * A simple HTML/CSS website hosted in the ``` /usr/share/nginx/html ``` directory on an EC2 instance.
   * Configured using Nginx to server static content.
2. Domain Configuration:
   * A custom domain (e.g., ``` www.vjaytech.site ```) purchased and configured.
   * DNS records (A Record) pointed to the public IP of the EC2 instance using the domain registrar or AWS Route 53.
3. Web Server Configuration:
   * Nginx configured to handle requests for the domain.
   * Created server block to define how traffic is handled for HTTP and HTTPS.
4. Securing Website with HTTPS:
   * Installed Certbot on the EC2 instance.
   * Generated and installed free SSL certificates using Let's Encrypt.
   * Auto-renewal setup via cron or systemd timers.


## **🔐 Security Considerations:**
   * Configured firewall rules (Security Groups) to allow HTTP (port 80) and HTTPS (port 443).
   * Restricted SSH (port 22) to specific IPs for better security.
   * Automatic renewal of SSL certificates every 60 days.


## **✅ Outcome:**
   * Static website is live and accessible using a custom domain name.
   * Connection is encrypted and secure using HTTPS.
   * SSL certificate is valid and auto-renewed using Certbot.


## **🚀 Skills Demonstrated:**
   * EC2 provisioning and Linux server management
   * Web server setup with Nginx
   * DNS and domain linking
   * SSL implementation with Let's Encrypt
   * Secure hosting best practices
