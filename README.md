# Ansible OpenVpn

Ansible OpenVpn repository contains roles, playbooks, and configurations to automate OpenVpn-related tasks using Ansible.

## Prerequisites

- Ansible 2.9 or higher
- Python 3.8 or higher
- Hashicorp Packer 

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/tamal-pension/ansible-openvpn.git
   cd ansible-api

## Command to run goldenimage.pkr.hcl locally

```bash
curl -O https://raw.githubusercontent.com/inqwise/ansible-automation-toolkit/default/packer/goldenimage.pkr.hcl && packer build --only=amazon-ebs.amzn2_x86 -var cpu_arch=x86 -var 'aws_profile=pension-stg' -var 'tag=latest' -var app=openvpn -var 'aws_region=eu-west-1' -var 'base_path=s3://bootstrap-pension-stg/playbooks' -var 'verbose=true' goldenimage.pkr.hcl
