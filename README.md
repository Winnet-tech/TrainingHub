## Project Overview 
The hub4Retail platform is a multi-page educational website designed to
support retail staff with training resources and organizational information.
It demonstrates the full process of deploying a web applicatiob on a cloud 
environment using industry-standard tools secure access methods and domain configuration

This project was created focusing on cloud deployment, web hosting,version control and webserver admninistration.

## Live Website
https://hub4retail.store/


## 🚀 Features

The platform includes the following full functional components:

## Website Pages 
**Home**  - hero banner ,introductory content visuals 
**About** Overview of the platform mission statement
**Courses**- training modules and short descriptions
**Contact**- details and structured contact section

## Technical Features
- Responsive layout with clean design
- Responsive navigation bar linking all pages
- Image intergration using royalty-free assets
- Custom CSS design
- Hosted on Microsoft  **Azure Ubuntu Virtual Machine**
- Secure access using **SSH key authentication** 
- Configured using  **Nginx** as a web server    
- Connected to a **custom domain: hub4retail.store**  
- Website located in:
  /var/www/hub4retail.store
-Secured using **Certbot SSL (HTTPS)**
-Github repository for version control
  
  ## 🛠 Technologies Used                     Components

- **HTML5** & - **CSS3**                       Front-end      
- **Nginx Web Server**
- **Ubuntu Linux**                             Cloud Hosting
- **SSH keys +Let’s Encrypt SSL Certificate**   Security
- **Git & GitHub**                               Version Control
- **Domain purchased from Namecheap**              

## PROJECT STRUCTURE 
hub4retail.store/
│── index.html
│── about.html
│── courses.html
│── contact.html
│── css/
│     └── style.css
│── images/
│     └── (hero banner + visuals)


 ## 💻 Deployment Steps Summary
1. Create and configure azure VM
- Created Ubuntu VM on Azure
- SSH Key pair generated and configured 
- Port 80 (HTTP) and 443 (HTTPS) opened

2.Connect to VM
  ssh -i yourkey.pem winnetbaibie@y20.94.41.52

3.Install and configure Nginx
  sudo apt update
  sudo apt install nginx
  set root directory and server block for domain

4.Upload Website Files 
/var/www/hub4retail.store

5.Domain setup (Namecheap)
Configured DNS:
A record @ ->VM public IP
A Record www ->VM public IP

6.Install SSL Certificate
sudo certbot --nginx -d hub4retail.store -d www.hub4retail.store

7.Github Version Control
git init
git add .
git commit -m "Initial project deployment"
git remote add origin <repo-url>
git push -u origin master 

## Screenshots
<img width="382" height="245" alt="image" src="https://github.com/user-attachments/assets/e3a475ed-5cb7-4ea1-a852-8b1f30f505dc" />
<img width="484" height="230" alt="image" src="https://github.com/user-attachments/assets/a7cc76dc-d785-4531-b135-e8668cc85dc5" />
<img width="450" height="200" alt="image" src="https://github.com/user-attachments/assets/96456061-e9bf-4328-891e-b9a7dfd29fc6" />
<img width="473" height="212" alt="image" src="https://github.com/user-attachments/assets/22f824ff-b366-4e4d-9062-278fe36185b2" />
<img width="375" height="227" alt="image" src="https://github.com/user-attachments/assets/5bb0fa48-7035-4642-b611-9677de83ca2f" />

## Security Considerations
- SSH password login disabled 
- Only key-based authentication used
- Firewall restricted ports
- Automated SSL certificate renewal enabled 


## Learning Outcomes 
- Through this project the following skills were demonstrated:
- Deploying web content on Azure 
- Configuring Nginx for custom domain hosting
- Managing DNS using Namecheap
- Using Git and Github for version control
- Implementing SSL certificates 
- Designing a functional multipage website 
- Understanding cloud security best practices 

## Author 
**Winnie Wambui**
GitHub Username: **winnetbaibie**
Student ID: 35589633




