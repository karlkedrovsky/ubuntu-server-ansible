# Ubuntu Ansible

Local Ubuntu server setup using ansible. This has only been tested using Ubuntu 20.04 on a raspberry pi.

Running against a remote raspberry pi (assumes the hostname is "raspberrypi4)

    ssh ubuntu@raspberrypi4  # changes the password
    ssh-copy-id -i ~/.ssh/id_ecdsa ubuntu@raspberrypi4
    ansible-playbook -i inventory -u ubuntu playbook.yml
    ansible-playbook -i inventory -u $USER playbook-user.yml

