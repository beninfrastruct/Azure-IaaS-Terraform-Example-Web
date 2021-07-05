# Azure-IaaS-Terraform-Example-Web
 Terraform-Example-Web
Project Details
Title
Provision Azure PaaS and IaaS resources to achieve a scalable deployment of Microsoft IIS web servers which are fronted by Azure Traffic Manager (for multi-region failover) and Azure Application Gateway (for single-region load balancing).

Description
Scalable Azure multi-region deployment of Microsoft IIS web servers across UK South and North Europe. Web servers are fronted by Azure Traffic Manager (for multi-region failover) and Azure Application Gateway (for single-region load balancing). Additionally, there is a NAT Gateway for outbound traffic, Key Vault for BitLocker disk encryption on the web servers, and storage accounts for boot diagnostics. Intention of this project is to demonstrate a multi-region deployment, which has an easily scalable web server instance count in each region using variables. Simply updating the variable will provision (or deprovision) the instances, disks, network interfaces, and relationship to the Application Gateway. The Microsoft IIS role is also automatically installed on the instances using an extension. This Terraform will provide the complete underlying infrastructure, allowing you to deploy your web application afterwards.