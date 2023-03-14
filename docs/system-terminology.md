# System Overview and Terminology

## Basics

### Directory Structure

Here's the directory structure of the init-5 repository:

```bash
init-5/
├── ansible/                             # Ansible playbooks for managing hosts remotely.
├── docker/                              # Contains two Docker images.
│   ├── ansible-runner/                  # A Docker image for running Ansible in a self-contained environment.
│   └── create-install-image/            # A Docker image for creating custom installation images.
├── docs/                                # Documentation and guidance for technical problems.
├── nixos/                               # A flake for NixOS configuration and home-manager setup.
│   └── profiles/                        # NixOS configuration based on machine type (host profile).
│       ├── profile1/                    # NixOS configuration of host profile1.
│       │   └── users/                   # Home-Manager configuration for each user on host profile1 as submodules
│       │       ├── user1/               # Home-Manager configuration for user1 as submodule.
│       │       └── user2/               # Home-Manager configuration for user2 as submodule.
│       └── profile2/                    # NixOS configuration of host profile1.
│           └── users/                   # Home-Manager configuration for each user on host profile2 as submodules
│               └── user1/               # Home-Manager configuration for user1 as submodule.
└── scripts/                             # Automation scripts for building and installing the configuration on a machine.
```

### Terminology

- `Profiles`: Refers to the different types of machines (e.g. web server, database server, etc.) that are defined in the NixOS configuration flake.
- `Hosts`: Refers to the individual machines that are managed with Ansible playbooks.
- `Users`: Refers to the individual user accounts that are defined in the NixOS configuration flake as submodules and managed with home-manager. Submoduling allows for easier sharing of home configurations between different profiles.

## Users and Profiles

### Profiles

- `raziel`: Personal Workstation
- `vorador`: Legacy Workstation
- `dumah`: Personal VPN
- `ariel`: Web Server
