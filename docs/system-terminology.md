# System Overview and Terminology

## Basics

### Directory Structure

The directory structure of the repository is as follows:
- `ansible/`: Ansible playbooks for managing hosts remotely.
- `docker/`: Contains two Docker images:
  - `ansible-runner`: A Docker image for running Ansible in a self-contained environment.
  - `create-install-image`: A Docker image for creating custom installation images.
- `docs`: Documentation and guidance for technical problems.
- `nixos/`: A flake for NixOS configuration and home-manager setup. It includes the configuration for all host types and users' homes.
- `scripts/`: Automation scripts for building and installing the configuration on a machine.

### Terminology

- `Profiles`: Refers to the different types of machines (e.g. web server, database server, etc.) that are defined in the NixOS configuration flake.
- `Hosts`: Refers to the individual machines that are managed with Ansible playbooks.
- `Users`: Refers to the individual user accounts that are defined in the NixOS configuration flake and managed with home-manager.

## Users and Profiles

### System Profiles

- `raziel`: Personal Workstation
- `vorador`: Legacy Workstation
- `dumah`: Personal VPN
- `ariel`: Web Server
