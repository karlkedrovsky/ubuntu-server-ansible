# Ubuntu Ansible

Ubuntu server setup using ansible. The intention is to set up the server to host applications using docker. This has only been tested using Ubuntu 20.04.

To run against a remote raspberry pi with a hostname of "raspberrypi4"

    ssh ubuntu@raspberrypi4  # changes the password
    ssh-copy-id -i ~/.ssh/id_ecdsa ubuntu@raspberrypi4
    ansible-playbook -i inventory.raspberrypi4 -u ubuntu --ask-vault-pass playbook.yml
    ansible-playbook -i inventory.raspberrypi4 -u $USER playbook-user.yml

To run against remote remote server with a hostname of "linode-web01-2004". This assumes a SSH key has been uploaded to your Linode profile.

    ansible-playbook -i inventory.linode -u root --ask-vault-pass playbook.yml
    ansible-playbook -i inventory.linode -u $USER playbook-user.yml

