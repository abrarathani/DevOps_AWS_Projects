## CI/CD Project-1 Overview

This project showcases a practical end-to-end DevOps CI/CD pipeline, automating the deployment of a web application on Amazon Web Services (AWS) using industry-standard open-source tools. The pipeline is designed to provide hands-on experience with continuous integration, continuous delivery, configuration management, and infrastructure automation.

**Key Features:**
- Demonstrates the integration of Git, GitHub, Jenkins, Ansible, and EC2 to automate the deployment workflow.
- Automates the installation and configuration of an Apache (httpd) web server on a Linux EC2 instance.
- Uses GitHub webhooks to trigger Jenkins builds on every code commit, ensuring continuous integration.
- Implements secure, passwordless SSH communication between Jenkins, Ansible, and deployment targets.
- Employs Ansible playbooks for reliable, repeatable server configuration and application deployment.
- Shows how to organize infrastructure code and scripts for easy automation and reproducibility.

**Pipeline Flow:**
1. A developer updates or adds an `index.html` file and pushes it to the GitHub repository.
2. GitHub, via webhook, notifies Jenkins of the code change.
3. Jenkins automatically pulls the latest code, performs build steps, and securely transfers the website artifact to the Ansible server.
4. Jenkins triggers an Ansible playbook execution over SSH.
5. The Ansible playbook installs and configures the Apache web server on a target EC2 instance, then deploys the latest website content.
6. The deployed website becomes available using the public IP of the web host EC2 instance.

**Learning Outcomes:**
- Understand the real-world application of CI/CD in cloud environments.
- Learn configuration and orchestration of Jenkins and Ansible for automated deployments.
- Practice secure automation using SSH keys.
- Get exposure to troubleshooting common DevOps issues, such as server storage and Jenkins node management.

This project is ideal for DevOps beginners, students, and professionals looking to strengthen their automation and cloud deployment skills with a hands-on example using widely adopted tools and AWS infrastructure.
