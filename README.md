# NSO Ansible Assignment

This project automates the deployment of a Python Flask application behind a HAproxy load balancer using Ansible.

## 🧩 Architecture

- **bastionNSO** — SSH jump host (with public IP)
- **haproxy** — Load balancer (with public IP)
- **devA / devB / devC** — Flask app servers (with private IP)

## ⚙️ Deployment

Run from local machine (with SSH config and keys set):

```bash
ansible-playbook -i hosts site.yaml

