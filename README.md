# Ansible Role for Installing Elastic Agent on EC2

This repository contains an Ansible role for installing Elastic Agent on an EC2 instance.

## Prerequisites

- Ansible installed on your local machine.
- An EC2 instance running.
- SSH access to the EC2 instance.

## Configuration

Update the `inventory.yml` file with the details of your EC2 instance:

```yaml
---
all:
  hosts:
    ec2_instance:
      ansible_host: <EC2_PUBLIC_IP>
      ansible_user: <EC2_USER>
      ansible_ssh_private_key_file: <EC2_PRIVATE_KEY_PATH>