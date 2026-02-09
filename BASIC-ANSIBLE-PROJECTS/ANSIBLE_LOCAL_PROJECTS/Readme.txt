Ansible Network Automation with Cisco DevNet Sandbox:

This project demonstrates basic network automation using Ansible on a local Linux system (WSL) and locally stores in GENERATED_CONFIG folder.

It covers interface configuration, routing and verification, and automation best practices like variables, loops, and idempotency(avoid duplicates).

Platform: WSL (linux)
Sandbox Type: local file generated
Access Method: SSH using Ansible `local`
Automation Tool: Ansible


Python Virtual Environment Setup:

Note: lastest version of Linux system will restrict global Python installs, we use a virtual environment.

Install required system packages:

sudo apt update
sudo apt install python3-venv python3-full -y

Create environment:

python3 -m venv venv    (create inside required project folder)
source venv/bin/activate
pip install ansible ansible-pylibssh (it will install all required packages)