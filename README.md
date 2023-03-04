# init-5: NixOS Configuration and Home-Manager Automation Tools

NixOS configuration and home-manager setup for managing multiple hosts and users, using flakes. It provides comprehensive automation tools, including documentation, automation scripts, a Docker image for creating custom installation images, and Ansible for managing hosts remotely.

## Directory Structure

The directory structure of the repository is as follows:
- `ansible/`: Ansible playbooks for managing hosts remotely.
- `docker/`: Contains two Docker images:
  - `ansible-runner`: A Docker image for running Ansible in a self-contained environment.
  - `create-install-image`: A Docker image for creating custom installation images.
- `docs`: Documentation and guidance for technical problems.
- `nixos/`: A flake for NixOS configuration and home-manager setup. It includes the configuration for all host types and users' homes.
- `scripts/`: Automation scripts for building and installing the configuration on a machine.

## Usage

1. Clone the repository.
```bash
git clone --recurse-submodules https://github.com/sdhlfqr/init-5.git
```
**Work in progress**: This section is a work in progress and will be updated soon with more detailed information on how to use this repository and its contents.


## Credits

This repository was created by [Sayf Dhu al-Faqar](https://github.com/sdhlfqr). Contributions are welcome and appreciated.
