# Ansible Learning Repository

This repository contains my hands-on practice and learning exercises with Ansible as part of my DevOps learning journey.

## About Configuration Management

Managing multiple servers manually can be repetitive and error-prone. Configuration Management tools help automate server provisioning, software installation, configuration updates, and service management across multiple machines.

Ansible is a push-based configuration management tool that communicates with target servers over SSH and does not require any agent installation on managed nodes.

## What I Learned

### Ansible Basics

* Installing and configuring Ansible
* Understanding inventory files
* Running ad-hoc commands
* Testing connectivity using the ping module

### Playbooks

* Creating and executing playbooks
* Understanding YAML syntax
* Working with tasks and modules

### Variables

* Defining variables in playbooks
* Using variables to make playbooks reusable

### Loops

* Creating multiple resources using loops
* Using variables with loops

### File and Directory Management

* Creating directories using the file module
* Managing file permissions and ownership
* Understanding idempotency

### Service Management

* Installing packages using playbooks
* Starting and stopping services
* Enabling services at boot

### Ansible Roles

* Creating reusable roles using `ansible-galaxy role init`
* Understanding role directory structure
* Organizing tasks, variables, handlers, and templates
* Executing roles through a site playbook

### Templates and Handlers

* Creating Jinja2 templates
* Deploying dynamic content
* Using handlers to restart services only when changes occur

### Troubleshooting

* Debugging playbook execution failures
* Investigating service issues using systemctl and journalctl
* Resolving port conflicts between Nginx and Apache

## Repository Structure

```text
learn-ansible/
├── first-playbook.yml
├── variable-playbook.yml
├── create-dir-playbook.yml
├── loop-playbook.yml
├── loop-var-playbook.yml
├── example3/
└── roles_exmaple/
    └── apacheWeb/
```

## Key Concepts Practiced

* Inventory Management
* Ad-hoc Commands
* Playbooks
* Tasks
* Variables
* Loops
* Modules
* Templates
* Handlers
* Roles
* Service Management
* Privilege Escalation (`become`)
* Idempotency

## Practical Work Completed

* Created inventory files for multiple servers
* Installed and managed Apache using Ansible
* Created directories using the file module
* Implemented loops and variables in playbooks
* Built a reusable Apache role
* Deployed template-based content
* Troubleshot Apache startup issues caused by an Nginx port conflict

## Goal

The goal of this repository is to build practical experience with Ansible and infrastructure automation while developing skills required for DevOps and Cloud Engineering roles.

This repository will continue to grow as I learn advanced Ansible topics such as Vault, Tags, Roles, Collections, and CI/CD integration.
