# Apache Web Server Role

This Ansible role installs and configures the Apache web server on Ubuntu hosts.

## Overview

The purpose of this role is to demonstrate how Ansible Roles can be used to organize automation code into reusable and maintainable components.

The role performs the following tasks:

* Installs the Apache web server
* Starts and enables the Apache service
* Deploys a sample web page using a Jinja2 template
* Uses variables for configuration
* Uses handlers to restart the service when configuration changes

## Role Structure

```text
apacheWeb/
├── defaults/
├── files/
├── handlers/
├── meta/
├── tasks/
├── templates/
├── tests/
├── vars/
└── README.md
```

## Concepts Practiced

* Ansible Roles
* Tasks
* Variables
* Templates (Jinja2)
* Handlers
* Service Management
* Idempotency

## Variables

Default variables can be found in:

```text
defaults/main.yml
```

Example:

```yaml
company_name: Kumara Technologies
```

## Usage

Example playbook:

```yaml
---
- name: Configure Apache Web Server
  hosts: all
  become: true

  roles:
    - apacheWeb
```

Run the playbook:

```bash
ansible-playbook -i inventory site.yml
```

## Learning Notes

While testing this role, Apache initially failed to start because Nginx was already using port 80 on the target servers. After stopping Nginx, the role executed successfully. This helped me understand how service conflicts can affect automation workflows and how to troubleshoot them using systemctl and journalctl.

## Future Improvements

* Configure virtual hosts
* Deploy custom website content
* Add SSL support
* Support multiple Linux distributions
* Publish the role to Ansible Galaxy
