# Smart Travel - Dynamic Cloud-Based Landing Page

## 🌍 Project Title
**The Future of Smart Travel**

## 💡 Project Overview
Smart Travel is a cloud-based landing page hosted on AWS EC2. It showcases the future of intelligent and personalized travel planning with a sleek design and professional bio. This project demonstrates cloud deployment, server setup, and frontend design using HTML/CSS.

## 📌 Live Site
**Public IP Address**: [http://3.253.35.85](http://3.253.35.85)

---

## 🚀 Steps to Deploy the Project

### 1. **Launched EC2 Instance on AWS**
- Selected **Ubuntu Server 24.04 LTS**
- Instance type: `t2.micro` (free tier)
- Created key pair: `smart-travel-key.pem`
- Configured security group: Allowed **SSH (22)**, **HTTP (80)**, and **HTTPS (443)**

### 2. **Connected to Instance via SSH**
```bash
ssh -i "smart-travel-key.pem" ubuntu@3.253.35.85
```
### 3. **Install and start nginx**
```bash
sudo apt update
sudo apt install nginx -y
```
### 4. **Upload Files to EC2 Server**
```bash
scp -i smart-travel-key.pem index.html style.css lydia.jpg smarttravel.PNG ubuntu@ec2-3-253-35-85.eu-west-1.compute.amazonaws.com:~
```
### 5. **Move Files to Web Directory**
```bash
sudo mv ~/index.html ~/style.css ~/lydia.jpg ~/smarttravel.PNG /var/www/html
```
### 6. **Configure Nginx**
```bash
sudo nano /etc/nginx/sites-available/default
root /var/www/html;
index index.html;
```
### 7. **Reload nginx**
sudo systemctl reload nginx
```
8. View landing page
Visit: http://3.253.35.85
```
## 📸 Screenshot
![Screenshot.png](C:\Users\Lydia\Pictures\Screenshots\screenshot.png)

🛠️ Tools & Technologies
Amazon EC2

Nginx

Ubuntu Linux

HTML & CSS

SSH & SCP


