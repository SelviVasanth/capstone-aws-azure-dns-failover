# capstone-aws-azure-dns-failover
Multi-cloud static web app deployment using Azure and AWS with VM-based load balancing and DNS failover via Azure Traffic Manager
## Project Overview

This capstone project demonstrates a resilient, multi-cloud architecture for a logistics company's static web application. It leverages virtual machines, load balancers, and Azure Traffic Manager to ensure high availability, global accessibility, and DNS-based failover across AWS and Azure.

## Architecture Summary

- **Azure Region**: VMs behind Azure Load Balancer, integrated with Traffic Manager
- **AWS Region**: EC2 instances behind Application Load Balancer
- **Traffic Manager**: Weighted routing between Azure and AWS endpoints
- **Failover Logic**: Health probes and DNS-based rerouting
- **Security**: NSG and SG rules for HTTP/SSH access

![Architecture Diagram](architecture-diagram.png)

## Technologies Used

- Azure: VM, VNet, Load Balancer, Traffic Manager
- AWS: EC2, VPC, ALB, Target Groups
- Networking: Subnets, Route Tables, Security Groups
- Monitoring: Health probes, DNS failover
- Documentation: Markdown, screenshots, cost modeling

## Repository Structure
capstone-aws-azure-dns-failover/
│
├── README.md                  # Project overview, architecture summary, and learning outcomes
├── architecture-diagram.png  # Annotated diagram of Azure and AWS setup
├── .gitignore                # Git tracking exclusions (Terraform, VSCode, etc.)
│
├── docs/                     # Write-ups and case study documentation
│   └── Write-Ups.pdf         # Detailed project rationale and deployment steps
│
├── screenshots/              # Portal setup, routing rules, VM config, and test results
│   └── *.png                 # Visual evidence of deployment and configuration
│
├── source-code/              # Scripts, templates, and provisioning logic
│   ├── azure/                # Azure VM setup, NSG rules, Traffic Manager config
│   └── aws/                  # AWS VPC, EC2, ALB, security groups
│
└── estimates/                # Cost modeling and BOM for Azure and AWS
    ├── azure-estimate.xlsx
    └── aws-estimate.xlsx
