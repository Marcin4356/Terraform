# Terraform

A collection of Terraform configurations and modules for Infrastructure as Code (IaC) practices.

## 📋 Description

This repository contains reusable Terraform modules and configurations for provisioning and managing cloud infrastructure. It demonstrates best practices in IaC, modularization, and state management.

## 🛠️ Tech Stack

- **Infrastructure as Code:** Terraform (HCL)
- **Cloud Providers:** AWS, Azure, GCP (configurable)
- **Version Control:** Git

## 📋 Prerequisites

- Terraform >= 1.0
- Cloud provider CLI configured (AWS CLI, Azure CLI, or Google Cloud SDK)
- Git

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Marcin4356/Terraform.git
cd Terraform
```

### 2. Initialize Terraform

```bash
terraform init
```

### 3. Review Infrastructure Plan

```bash
terraform plan
```

### 4. Apply Configuration

```bash
terraform apply
```

## 📁 Project Structure

```
Terraform/
├── modules/
│   ├── networking/
│   ├── compute/
│   ├── storage/
│   └── security/
├── environments/
│   ├── dev/
│   ├── staging/
│   └── production/
├── main.tf
├── variables.tf
├── outputs.tf
├── terraform.tfvars
└── README.md
```

## 🔧 Key Features

- ✅ Modular architecture for reusability
- ✅ Environment-based configuration (dev, staging, prod)
- ✅ Comprehensive variable definitions
- ✅ State management with remote backends
- ✅ Security best practices

## 📝 Common Commands

```bash
# Validate configuration
terraform validate

# Format code
terraform fmt -recursive

# Plan changes
terraform plan -out=tfplan

# Apply changes
terraform apply tfplan

# Destroy resources
terraform destroy
```

## 📚 Resources

- [Terraform Documentation](https://www.terraform.io/docs)
- [Terraform Registry](https://registry.terraform.io/)
- [Terraform Best Practices](https://www.terraform.io/language)

## 📝 License

This project is open source and available under the MIT License.

## 👤 Author

**Marcin4356** - [GitHub Profile](https://github.com/Marcin4356)

---

*Last updated: 2026-04-28*
