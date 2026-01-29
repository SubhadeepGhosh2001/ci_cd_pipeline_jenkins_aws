# CI/CD Pipeline using Jenkins and AWS 🚀

This project demonstrates a complete **CI/CD (Continuous Integration & Continuous Deployment) pipeline** using **Jenkins** and **AWS EC2**.  
Whenever code is pushed to GitHub, Jenkins automatically pulls the changes, builds the project, and deploys it to an EC2 instance.

This setup reflects a real-world DevOps workflow used in production environments.

---

## 🧠 CI/CD Concepts Covered
- Continuous Integration (CI)
- Continuous Deployment (CD)
- Jenkins Pipelines
- GitHub Webhooks
- SSH-based deployment
- AWS EC2 server management

---

## 🛠️ Tech Stack
- **Jenkins** – CI/CD automation server  
- **GitHub** – Source code management  
- **AWS EC2 (Ubuntu)** – Deployment server  
- **SSH** – Secure remote access  
- **Node.js / Web App** – Sample application  

---

## ⚙️ Architecture Overview


---

## 🔄 CI/CD Workflow

1. Developer pushes code to GitHub
2. GitHub triggers Jenkins using a webhook
3. Jenkins pulls the latest code
4. Jenkins builds the project
5. Jenkins connects to EC2 using SSH
6. Application is deployed automatically

---

## 📁 Jenkins Pipeline Stages

- **Checkout** – Pull code from GitHub
- **Build** – Install dependencies / build app
- **Test (optional)** – Run tests
- **Deploy** – Copy files and restart application on EC2

---

## 🔐 Security Practices
- SSH key-based authentication
- Jenkins credentials management
- Restricted permissions on PEM files
- No hardcoded secrets in repository

---

## 🚀 How to Run This Project

### 1️⃣ Setup AWS EC2
- Launch Ubuntu EC2 instance
- Open ports (22, 8080)
- Configure SSH access

### 2️⃣ Setup Jenkins
- Install Jenkins on local machine or EC2
- Configure GitHub credentials
- Add SSH private key to Jenkins credentials

### 3️⃣ Configure GitHub Webhook
- Add Jenkins webhook to GitHub repository

### 4️⃣ Create Jenkins Pipeline
- Define pipeline stages using Jenkinsfile
- Configure build & deploy steps

---

## 📌 Outcome
- Fully automated deployment
- Faster feedback loop
- Reduced manual errors
- Production-like CI/CD experience

---

## 📚 Learning Outcome
This project helped me understand:
- Real-world CI/CD pipeline design
- Jenkins pipeline configuration
- AWS server deployment
- Secure automation practices

---

## 👨‍💻 Author
**Subhadeep Ghosh**  
MCA | DevOps & Cloud Enthusiast  
# ci_cd_pipeline_jenkins_aws
