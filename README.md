# Decode Lab - AWS EC2 Static Website

## 📌 Project Overview

This project demonstrates the deployment of a static website using **Amazon EC2**.

The website is created using **HTML and CSS** and hosted on an AWS EC2 cloud server. The objective of this project is to understand the basic process of deploying and accessing a website using cloud computing services.

## 🏗️ Architecture

**Internet → HTTP : 80 → AWS Security Group → Amazon EC2 → Web Server → Static HTML/CSS Website**

---

## ☁️ AWS Services Used

* Amazon EC2
* EC2 Key Pair
* Security Groups

---

## 🛠️ Technologies Used

* HTML5
* CSS3
* Linux
* AWS EC2
* SSH
* GitHub

---



## 🚀 Deployment Process

### 1. Launch EC2 Instance

Created an AWS EC2 instance and selected a Linux-based operating system.

### 2. Configure Security Group

Configured the security group to allow:

* SSH (Port 22)
* HTTP (Port 80)

### 3. Connect to EC2

Connected to the EC2 instance using SSH and the EC2 key pair.

### 4. Configure Web Server

Installed and configured a web server on the EC2 instance to serve the static website.

### 5. Upload Website Files

Uploaded the website files to the web server directory.

The project contains:

* `index.html` – Main webpage
* `style.css` – Website styling

### 6. Access the Website

The website can be accessed through the **public IPv4 address of the EC2 instance** using a web browser.

---

## 📂 Project Structure

```
DecodeLabs-EC2-Static-Website/
│
├── index.html
├── style.css
└── README.md

```

---

## 🎯 Project Objective

The main objective of this project is to gain practical experience with:

* Cloud computing
* AWS EC2
* Linux servers
* Security Groups
* SSH
* Web server configuration
* Static website deployment

---

## 📚 What I Learned

Through this project, I learned how to:

* Launch and configure an EC2 instance
* Connect to a Linux server using SSH
* Configure AWS Security Groups
* Deploy a static website on a cloud server
* Configure a web server
* Access a website using an EC2 public IP
* Understand the basic workflow of cloud-based website hosting

\

---

## ✨ Features

* Responsive static website
* HTML-based website structure
* CSS-based styling
* Cloud deployment using AWS EC2
* Ubuntu server environment
* Apache web server
* SSH-based server management
* Publicly accessible website





⭐ If you found this project useful, consider giving the repository a **star**!
