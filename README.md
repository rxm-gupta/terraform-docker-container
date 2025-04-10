# 🚀 Infrastructure as Code (IaC) with Terraform

## 📌 Objective
Provision a local **Docker container** using **Terraform**, demonstrating Infrastructure as Code (IaC) principles.

---

## 🛠️ Tools Used
- **Terraform** (v1.0+)
- **Docker** (locally installed)

---

## 📁 Project Structure

terraform-docker-container/  
├── main.tf                # Terraform configuration file  
├── terraform.lock.hcl     # Provider version lock file  
├── .gitignore             # Excludes sensitive and auto-generated files  
├── terraform.log          # Terraform command execution logs  
└── README.md              # Project documentation  

---

## ✅ Prerequisites

Install and run the following:  
- **Docker**: https://www.docker.com/products/docker-desktop  
- **Terraform**: https://developer.hashicorp.com/terraform/downloads  

Verify installations:  
```bash
docker --version  
terraform --version
```

---

## ⚙️ Steps to Run the Project

**Clone this Repository**  
```bash
git clone https://github.com/rxm-gupta/terraform-docker-container.git  
cd terraform-docker-container
``` 
---

**Initialize Terraform**

```bash
terraform init
```
---

**Preview Changes**

```bash
terraform plan
```
---

**Apply Configuration**

```bash
terraform apply -auto-approve
```
--- 

**Access the App**

Visit in your browser:
```bash
http://localhost:8082
```
You should see the default NGINX welcome page.

---

Verify Container is Running
```bash
docker ps
```
---

**🔁 Destroy the Infrastructure**
After testing, clean up the resources:

```bash
terraform destroy -auto-approve
```
