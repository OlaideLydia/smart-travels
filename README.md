# Smart Travel - Dynamic Cloud-Based Landing Page

## 🌍 Project Title
**The Future of Smart Travel**

---

## 💡 Project Overview
Smart Travel is a cloud-hosted, responsive landing page created to demonstrate real-world cloud deployment skills. This project simulates a travel startup's online presence using HTML, CSS, and Nginx on an AWS EC2 instance. It includes a pitch, bio, and animations for professional presentation.

---

## 📌 Live Site
**Public IP Address:**  
[http://3.253.35.85](http://3.253.35.85)

---

## 🚀 Project Setup & Deployment Steps

### ✅ 1. Launch EC2 Instance on AWS
- Selected **Ubuntu Server 24.04 LTS**
- Instance type: **t2.micro**
- Created key pair: `smart-travel-key.pem`
- Opened ports: **SSH (22), HTTP (80), HTTPS (443)**

### ✅ 2. Connect to EC2 via SSH
```bash
ssh -i "smart-travel-key.pem" ubuntu@ec2-3-253-35-85.eu-west-1.compute.amazonaws.com
