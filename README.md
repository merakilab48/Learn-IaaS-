# Infrastructure as a Service (IaaS) Learning Project

## Overview
This project will guide you through deploying a foundational virtual machine (VM) in a cloud environment. You’ll learn to create, secure, and configure the VM through both UI and CLI, and eventually automate the deployment using Infrastructure as Code (IaC).

---

## Steps

### Foundational Virtual Machine Setup
- [ ] **Find the cheapest VM instance**  
  Identify the lowest-cost virtual machine on your cloud provider (e.g., AWS, Azure, Google Cloud).
  
- [ ] **Deploy the VM via UI**  
  Launch the VM using the cloud provider's web console (e.g., Azure Portal, AWS Console).
  
- [ ] **Deploy the VM via CLI**  
  Learn the CLI command to deploy the same VM instance (e.g., `az vm create` for Azure).
  
  - [ ] **SSH after creation**  
    Configure SSH access so you can connect directly to the VM once it's deployed.

### Security & Networking Configuration
- [ ] **Allow SSH only from your IP**  
  Set up a Network Security Group (NSG) or equivalent to allow SSH access exclusively from your current IP.
  
- [ ] **Enable auto power-off**  
  Configure auto-shutdown for the VM at a specific time daily.

### Command Configuration
- [ ] **Turn VM on/off via CLI**  
  Familiarize yourself with the CLI commands to power on and off the VM manually.

---

### Automation & Infrastructure as Code (IaC)
- [ ] **Create Bash/Powershell script**  
  Create a script with the necessary CLI commands to automate VM deployment.
  
- [ ] **Translate to Infrastructure as Code**  
  Create an IaC template (e.g., `main.tf` for Terraform or `main.bicep` for Azure) to automatically deploy the VM with all configurations.

  - [ ] **Store SSH Public Key in Key Vault**  
    Save your SSH public key in a secure location like Key Vault, ensuring secure access for IaC deployment.

### Final Configuration
- [ ] **Configure deployment details**  
  Make sure your IaC template includes the following configurations:
    - Auto-shutdown settings
    - SSH access restriction to your IP
    - Appropriate disk and storage configurations
  
- [ ] **Run deployment and validate**  
  Use your IaC template to deploy the VM and verify that all configurations have been applied successfully.

---

## Additional Resources
- **Paper Recommendation:** _The Ideal vs the Real: Revisiting the History of Virtual Machines and Containers_  
- **Newsletter Subscription:** Subscribe to keep up with further resources and updates on this project.

---

## Next Steps
After completing this foundational setup, you can expand by:
- Deploying multiple VMs to configure communication between them
- Setting up basic networking, such as load balancers
- Experimenting with other cloud services and advanced configurations
