# 🚀 Automating Multi-Tier Java Web Application Deployment Using Ansible

## 📌 Project Overview
This project automates the deployment of a **multi-tier Java web application** on a local infrastructure using **Ansible Playbooks and Roles**. By leveraging **Vagrant, VirtualBox, and Ansible**, we ensure a fully automated, consistent, and scalable deployment process.

## 🎯 Purpose
- **Eliminate manual configurations** by automating provisioning and setup.
- **Ensure consistency & scalability** across multiple environments.
- **Reduce deployment time** from hours to minutes.
- **Implement modular and reusable Ansible Roles** for maintainability.

## 🔧 Tech Stack & Tools Used
| Tool          | Purpose                                         |
|--------------|-----------------------------------------------|
| **Vagrant**  | Automates virtual machine creation            |
| **VirtualBox** | Runs virtual machines                        |
| **Ansible**  | Automates configuration management            |
| **Tomcat**   | Java application server                        |
| **Nginx**    | Web server & reverse proxy                    |
| **RabbitMQ** | Message broker for async communication        |
| **Memcached** | Caching layer for performance                 |
| **MySQL**    | Relational database for data storage         |
| **Maven**    | Build automation tool for Java projects       |
| **Git**      | Version control system                        |

## 🏗️ Architecture
The project consists of multiple virtual machines running:
- **Web Server (Nginx)**
- **Application Server (Tomcat)**
- **Database Server (MySQL)**
- **Message Broker (RabbitMQ)**
- **Cache Server (Memcached)**

![Project Architecture](./architecture.gif)![2025-02-1704-18-02online-video-cutter com-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/b76638a2-25cc-4408-b60a-da4572af7aeb)



## 📌 Setup Instructions

### 1️⃣ Prerequisites
Ensure you have:
- **Vagrant & VirtualBox Installed** → [Download Vagrant](https://www.vagrantup.com/downloads)
- **Ansible Installed** → [Install Guide](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)
- **Git Installed** → [Download Git](https://git-scm.com/downloads)

### 2️⃣ Clone This Repository
```sh
$ git clone https://github.com/yourusername/Ansible-MultiTier-Deployment.git](https://github.com/MohamedElweza/Automating-Multi-Tier-Java-Web-Application-Deployment-with-Ansible.git
```

### 3️⃣ Start Virtual Machines
Run the following command to create and start all VMs:
```sh
$ vagrant up
```

### 4️⃣ Run Ansible Playbook
Once VMs are up, configure all services with Ansible:
```sh
$ ansible-playbook -i inventory site.yml
```

## 📂 Project Structure
```
Ansible-MultiTier-Deployment/
│── ansible/
│   ├── inventory  # Hosts file
│   ├── site.yml   # Main playbook
|   ├── ansible.cfg 
│   ├── roles/
│   │   ├── nginx/
│   │   ├── tomcat/
│   │   ├── mysql/
│   │   ├── rabbitmq/
│   │   ├── memcached/
│   │   ├── common/
```

## 🔥 Security Best Practices
✅ Each service is assigned a **separate Ansible Role** for better **modularity & reusability**.
✅ **Firewalls & Security Groups** are configured for **least privilege access**.
✅ **Ansible Vault** can be used to securely manage sensitive configurations.

## 🚀 Next Steps
In the next phase, we will:
- **Deploy this architecture on AWS using Terraform.**
- **Containerize the application with Docker & Kubernetes.**
- **Implement CI/CD pipelines for automation.**

## 👨‍💻 Contributors
- **Mohamed Elweza**
- **Nader Ashour**

---

📌 **Follow this repository for updates!**
✅ If you found this useful, don't forget to **star ⭐ the repo**!

💬 Feel free to open issues or contribute to improve this setup!
