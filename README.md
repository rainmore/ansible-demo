Ansible 
=======

python2 and ssh are required on remote

ssh-copy-id -i is required on local


# WorkStation Setup



Required software

OPENSSL, Python

# Remove machine

Required software

OPENSSL, Python

# Example 1
Run a command to all servers
```
ansible -m shell -a "hostname" all
```
equal to
```
ansible -m command -a "hostname" all
```
# Example 2
Run a script to a single server with specified the `hosts` file
```
ansible vm001 -i hosts -m script -a "vm001.sh"
```

# Playbook

Prompt
```
ansible-playbook -K playbook.yml
```

Check syntax
```
ansible-playbook --syntax-check playbook.yml
```
