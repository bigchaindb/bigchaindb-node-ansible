## Bigchaindb ansible deployment recipes

This repository contains a collection of ansible playbooks for quick bigchaindb node deployment and orchestration.

### What can be done

- Installation of BigchainDB
    - Adding and configuring users
    - Mongodb installation
    - Specified python version installation
    - Tendermint installation
    - BigchainDB installatin and configuration
    - Enabling and activating services
    - TODO Nginx configuration
- TODO Connecting nodes into a network
- TODO Adding/removing validators

### Limitations

- Requires ssh connection to a sudoer/root
- Currently works/tested on Ubuntu 18.04 only
        

### How to use

1. Inspect ./vars/install-config.yml and edit settings if required.
2. Add list of hosts to ./hosts/all file.
2. cd into playbook directory.
3. run with `ansible-playbook install.yml -i hosts/all --extra-vars "top_dir=$(pwd)"` in bash shell.
4. Wait for all plays to complete

Bigchaindb should be now available on port 9984.

### Other notes

This is basically a collection of shell snippets, ansible people are more then welcome to pick at it.
