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

[View Architecture Diagram](screenshots/Architecture-Diagram.png)


## Technologies Used

- Azure: VM, VNet, Load Balancer, Traffic Manager
- AWS: EC2, VPC, ALB, Target Groups
- Networking: Subnets, Route Tables, Security Groups
- Monitoring: Health probes, DNS failover
- Documentation: Markdown, screenshots, cost modeling
