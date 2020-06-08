# Ubuntu Ansible

Local Ubuntu workstation setup using ansible. This has only been tested using Xubuntu 19.10.

Make sure everything is up to date.

    sudo apt update
    sudo apt upgrade

Use the latest version of ansible.

    sudo apt-add-repository ppa:ansible/ansible
    sudo apt update
    sudo apt install ansible

Install git

    sudo apt install git

Run the installation.

    sudo ansible-pull -U https://github.com/karlkedrovsky/ubuntu-server-ansible.git
