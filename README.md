# devops-jenkins-terraform-docker
# DevOps Mini Project: Jenkins + Terraform + Docker

## 🧱 Stack Used
- Jenkins for CI/CD
- Docker for containerizing the app
- Terraform to provision AWS EC2

## 🚀 Workflow
1. Jenkins builds Docker image from Flask app
2. Pushes to DockerHub
3. Terraform provisions EC2 and runs Docker container

## 🔧 Prerequisites
- AWS account with access keys
- DockerHub account
- Jenkins with Docker & Terraform installed
- A key pair created in AWS (`.pem` file)

## 📦 Build Steps
1. Clone this repo
2. Update:
   - Docker image name in `Jenkinsfile` and `main.tf`
   - AWS key pair in `main.tf`
3. Create a Jenkins Pipeline pointing to this GitHub repo
4. Add DockerHub credentials in Jenkins (`dockerhub-credentials`)
5. Run the pipeline!

## 🌐 Access App
Visit the public IP of the EC2 instance after provisioning (port 80)

---
