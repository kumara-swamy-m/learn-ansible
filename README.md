# Ansible 

This repository contains my hands-on practice and learning exercises with Ansible.

## About Configuration Management

Managing multiple servers manually can be time-consuming and error-prone. Configuration Management tools help automate server configuration, software installation, updates, and maintenance across multiple machines from a central location.

Ansible is a push-based configuration management tool that uses SSH to communicate with Linux servers and does not require any agent installation on target machines.

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
* Understanding idempotency in Ansible

### Service Management

* Installing and managing services
* Starting and stopping services using playbooks

## Repository Structure

* `first-playbook.yml` – Basic playbook examples
* `variable-playbook.yml` – Working with variables
* `create-dir-playbook.yml` – Directory creation using the file module
* `loop-playbook.yml` – Loop examples
* `loop-var-playbook.yml` – Loops with variables
* `example3/` – Additional practice examples

## Key Concepts Practiced

* Inventory Management
* Playbooks
* Tasks
* Variables
* Loops
* Modules
* Privilege Escalation (`become`)
* Idempotency

## Goal

The goal of this repository is to build practical experience with Ansible and infrastructure automation as part of my DevOps learning journey.
