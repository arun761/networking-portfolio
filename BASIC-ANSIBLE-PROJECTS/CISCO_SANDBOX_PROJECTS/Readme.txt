Ansible Network Automation with Cisco DevNet Sandbox:

This project demonstrates basic network automation using Ansible on a Cisco router hosted in the Cisco DevNet Always-On Sandbox.

It covers interface configuration, routing, DHCP, OSPF, verification, and automation best practices like variables, loops, and idempotency(avoid duplicates).

Platform: Cisco Catalyst 8000V (IOS-XE)
Sandbox Type: Cisco DevNet Always-On Sandbox
Access Method: SSH using Ansible `network_cli`
Automation Tool: Ansible

The sandbox is cloud-hosted and resets every 2 days , so all configurations are rebuilt using automation playbooks.

Python Virtual Environment Setup:

Note: lastest version of Linux system will restrict global Python installs, we use a virtual environment.

Install required system packages:

sudo apt update
sudo apt install python3-venv python3-full -y

Create environment:

python3 -m venv venv    (create inside required project folder)
source venv/bin/activate
pip install ansible ansible-pylibssh (will will install all required packages)