# Terraform AWS EC2

A Terraform configuration for provisioning a small AWS environment containing a VPC, subnet, routing, security group, SSH key pair, and an EC2 instance.

## Architecture

```
AWS
└── VPC
    └── Subnet
        └── EC2 instance
            └── Amazon Linux 2023
```

## Technologies

- Terraform
- AWS
- Amazon VPC
- Amazon EC2
- HCL
- Amazon Linux 2023

## Infrastructure

The configuration defines:

- VPC with configurable CIDR
- subnet with configurable availability zone
- Internet Gateway
- route table with default internet route
- security group
- EC2 SSH key pair
- EC2 instance
- automatic lookup of the latest Amazon Linux 2023 AMI
- Terraform outputs for the AMI ID and public IP

The security group allows SSH from the configured source address and exposes port 8080.

## Variables

The configuration expects values for:

- VPC CIDR
- subnet CIDR
- availability zone
- environment prefix
- allowed SSH source
- EC2 instance type
- public key path

## Usage

```bash
terraform init
terraform fmt
terraform validate
terraform plan
terraform apply
```

Remove the infrastructure when it is no longer needed:

```bash
terraform destroy
```

This is a personal Infrastructure as Code lab for AWS networking and EC2 provisioning.
