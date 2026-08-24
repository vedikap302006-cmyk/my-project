# 🌐 AWS EC2 Static Website Deployment

## 📌 Project Overview

This project demonstrates the deployment of a **static website using Amazon EC2**.

The website is developed using **HTML5 and CSS3** and hosted on an **AWS EC2 Linux server** using a web server. The project provides practical experience with cloud computing, Linux server administration, SSH connectivity, AWS Security Groups, and website deployment.

The main goal is to understand how a website can be hosted on a cloud-based virtual server and accessed through its public IP address.

---

## 🏗️ Architecture

**Internet → HTTP (Port 80) → AWS Security Group → Amazon EC2 → Web Server → HTML/CSS Website**

---

## ☁️ AWS Services Used

* **Amazon EC2** – Virtual cloud server used to host the website
* **EC2 Key Pair** – Used for secure SSH authentication
* **Security Groups** – Used to control inbound and outbound network traffic

---

## 🛠️ Technologies Used

* HTML5
* CSS3
* Linux / Ubuntu
* Amazon EC2
* Apache Web Server
* SSH
* GitHub

---

## 🔐 Security Group Configuration

### Inbound Rules

| Protocol | Port | Source    | Purpose                    |
| -------- | ---: | --------- | -------------------------- |
| TCP      |   22 | My IP     | SSH administration         |
| TCP      |   80 | 0.0.0.0/0 | Public HTTP website access |

### Outbound Rules

| Protocol    | Port | Destination | Purpose                |
| ----------- | ---: | ----------- | ---------------------- |
| All Traffic |  All | 0.0.0.0/0   | Allow outbound traffic |

### 🔒 Security

SSH access on **Port 22** is restricted to my IP address rather than allowing SSH access from the entire internet.

HTTP traffic on **Port 80** is publicly accessible so that users can open the website through a web browser.

---

## 🚀 Deployment Process

### 1. Launch EC2 Instance

Created an Amazon EC2 instance using a Linux-based operating system.

The instance provides the virtual server environment required to host the website.

---

### 2. Configure Security Group

Configured the EC2 Security Group with the following inbound rules:

* **SSH – Port 22** → My IP
* **HTTP – Port 80** → Anywhere

This allows secure server administration while making the website publicly accessible.

---

### 3. Connect to EC2 Using SSH

Connected to the EC2 instance using **SSH** and the EC2 key pair.

SSH provides a secure way to access and manage the Linux server remotely.

---

### 4. Install Web Server

Installed and configured the **Apache web server** on the EC2 instance.

Apache is responsible for receiving HTTP requests and delivering the website files to users' browsers.

Example commands:

```bash
sudo apt update
sudo apt install apache2 -y
sudo systemctl start apache2
sudo systemctl enable apache2
```

---

### 5. Upload Website Files

Uploaded the static website files to the Apache web server directory.

The main website files include:

```text
index.html
style.css
```

The files were placed inside the Apache web directory:

```text
/var/www/html/
```

---

### 6. Configure Website

The `index.html` file contains the structure and content of the website, while `style.css` is used to control the website's appearance and layout.

Example project structure:

```text
AWS-EC2-Static-Website/
│
├── index.html
├── style.css
└── README.md
```

---

### 7. Access the Website

After configuring the web server and security group, the website can be accessed through the **Public IPv4 Address** of the EC2 instance.

Example:

```text
http://YOUR-EC2-PUBLIC-IP
```

The public IP can be entered into a web browser to view the deployed website.

---

## 📂 Project Structure

```text
AWS-EC2-Static-Website/
│
├── index.html        # Main webpage
├── style.css         # Website styling
└── README.md         # Project documentation
```

---

## 🎯 Project Objectives

The main objectives of this project are to gain practical knowledge of:

* Cloud computing
* Amazon EC2
* Linux server administration
* Apache web server
* SSH
* AWS Security Groups
* HTTP and network ports
* Static website deployment
* GitHub project management

---

## 📚 What I Learned

Through this project, I learned how to:

* Launch an EC2 instance on AWS
* Configure an AWS Security Group
* Connect to a Linux server using SSH
* Install and configure Apache
* Upload HTML and CSS files to a cloud server
* Host a static website on EC2
* Configure HTTP access through Port 80
* Access a website using an EC2 Public IPv4 address
* Understand the basic workflow of cloud-based web hosting

---

## 💡 Key Learning

This project helped me understand the basic workflow of deploying a website on the cloud:

**Create EC2 → Configure Security Group → Connect using SSH → Install Apache → Upload Website → Open Public IP → Website Goes Live 🚀**

---

## 📸 Project Output

The final output is a live static website hosted on an **AWS EC2 Linux server** and accessible through the EC2 instance's public IPv4 address.

---

## 🔗 Project Links

**Live Website:**
`Add your EC2 Public IPv4 website link here`

**GitHub Repository:**
`Add your GitHub repository link here`

---

## 👩‍💻 Author

**Your Name**

Cloud Computing / AWS Project

---

## ⭐ Conclusion

This project provided hands-on experience with **AWS EC2, Linux, Apache, SSH, Security Groups, and static website hosting**. It demonstrates how cloud infrastructure can be used to deploy and make a website accessible over the internet.

The project is a practical introduction to **cloud-based web hosting and server management**.
# my-project
