# Beginner Realistic Ansible Setup

This is a simplified but realistic version of the Hadoop–Kerberos–OpenLDAP Ansible project.

## Steps to Run

1. Install Ansible (example for Ubuntu/Debian):
   ```bash
   sudo apt update && sudo apt install -y ansible
   ```

2. Run the playbook:
   ```bash
   ansible-playbook -i inventory.ini site.yaml
   ```

## What happens

- **OpenLDAP**: Installs slapd and adds a base DN.
- **Kerberos**: Installs krb5-kdc and admin server with minimal configs.
- **SSH**: Ensures OpenSSH is installed and running.
- **Hadoop**: Creates dummy configs under /opt/hadoop.

This lets you practice with roles, templates, handlers, and defaults in a real-world structure.
